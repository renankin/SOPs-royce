# SOPs for SLM 280 system

## General Safety Concepts for the SLM system

* Only qualified personnel are authorized to operate the SLM system. Qualified personnel are those that have been instructed by a SLM-authorized service technician. All required training must be completed before being considered qualified to operate the SLM system.
* Technical staff operating the SLM 280 system must follow the operating instructions, the safety data sheets, and the process parameters established for the system.
* Technical staff must observe and follow the safety warnings posted in the laboratory and provided in the manuals and other safety documentation. 
* Technical staff must wear the required protective equipment appropriate, and risk assess the activity before carrying out any work. Depending on the activity (see the specific standard operating procedures), personal protective equipment (PPE) includes:
  - Powered air-purifying respirator (EN166 and FFP3 EN149)
  - Anti-static safety shoes (EN20344) used in conjunction with a ground anti-static floor pad
  - Safety shoes with steel/composite toe caps (EN20345)
  - Single use nitrile gloves (EN374)
  - Anti-static coveralls (EN1149-5)
* The SLM 280 system has several built-in safety features (e.g., chamber door interlocks, room air monitoring, inert gas monitoring, laser readiness indicator, laser-safe window, grounded system components, emergency stop circuit, safe stop laser, emergency stop switch laser, covers to protect against laser radiation). Technical staff must not disable or override the built-in safety features of the system.
* Flammable materials should not be stored in the working area around the machine. Sources of ignition and electrostatic discharge should be eliminated and avoided as much as possible.
* Working with metal powder requires several safety precautions, including respiratory protection, protective gloves, non-sparking tools and equipment, anti-static grounding, and careful manipulation to prevent dust clouds. See specific procedures below for working with metal powders.

## Switching on the machine

* Turn the main switch for the machine to the “ON” position.
* As soon as the SLM logo and versions of Scout and TLM/LMC are displayed on the SPS monitor, a blink dot will follow. The user needs to press the [Reset] button when the dot is blinking.
* The control PC starts automatically, and you need to log in to the PC. Password is “slm280hl”
* Start the MCS software.
* Carry out homing on the recoater (Manual control → Motor → Recoater → Reset).
* Press the [Homing] button to place the recoater in the home position.
* Move the build platform to position [Top]. (Manual control → Motor → Platform → Top).
* Make sure that the laser control unit selector switch is in the “REM” position.

## Preparation of Build Platform and Substrate plate

* This procedure assumes that the chamber has been completely cleaned, if this is not the case follow Cleaning Up the Process Chamber.
* Prior to inserting the build platform into the chamber, clean off excess machine oils from the substrate plate using paper towels with IPA.
* Safety shoes with steel/composite toe caps (EN20345) are necessary when lifting or moving heavy substrate plates. In addition, the lifting trolley supplied by SLM is available for use when large parts are fabricated on the substrate plate. 
* When mounting the substrate plate, first insert the bolts loosely (do not tighten). Close the build chamber and cover barrier and press the reset button. Turn on the build platform heating using the MCS control program (Manual control → Gas & Temp → Platform Heating). Tighten the bolts only after the build platform temperature reaches 80 ºC (takes about 20 min from room temperature). 
* Prior to the start of each build, the upper edge of the substrate plate must be levelled and positioned to have the appropriate relation with the recoating blade. Level the build platform according to the instructions provided in the SLM operations manual (p. 133).
* First, it is roughly aligned with a straightedge or square (without powder) to check whether the substrate plate is flush with the base plate of the process chamber:
1. Move the plate slightly higher than necessary and press the button ↓ (Stepwise) using 0.1 increments. It is important to approach the final position of the build platform from above as the reverse backlash of the shaft will be compensated and will prevent the platform from dropping later.
2. After every increment, open the process chamber and check whether the substrate is flush with the base plate of the chamber.
3. If necessary, repeat the steps above until a satisfactory height is reached.
4. After finding a satisfactory position, the button “Zero Setting” can be pressed.
* The fine adjustment of the substrate plate height is carried out with powder:
1. The process chamber can be first flood with argon to protect the powder that will be released into the chamber. To do this go to (Manual control → Gas & Temp → Flood Inlet and Outlet “Open”).  Wait until Oxygen level in sensors 1 & 2 is below 0.5 % and press “Close” in Flood Inlet and Outlet. 
2. Next, reset the recoater position if enabled (Manual control → Motor → Recoater → Reset) and press the “Homing” button to place the recoater in the home position.
3. Next, home the powder loader (Manual control → Powder Loader → Homing) and enter the value 35 and press enter. The recoater is filled with powder.
4. Press the “Recoat Layer” button.
5. Now enter value -2 in the Platform Target position and press Enter. Wait until the movement is finished. And then enter value -0.1 and press Enter again. Press “Zero Position” to save the new zero setting.
6. Press the “Recoat Layer” button.
7. Carry out a visual inspection through the laser safety glass of the process chamber door. The substrate plate must clearly shine through the thin layer of powder, and the holes of the heads must be covered with powder. If this is not the case. Repeat steps 5-7

## Implementing the Build Process

* Following the preparation of build chamber and substrate plate (Preparation of Build Platform and Substrate plate) and creating the .SLM file with Materialise, the build process can start.
* Make sure that the main tank is filled with sufficient powder, if not follow procedure detailed in Handling and Filling Metal Powder into Hoppers.
* Download the .SLM file to the SLM 280 using the USB port in the front panel of the machine. The location to load the files into the machine is “DATA(:D)\Jobs & Parts”.
* Press “Open File” icon in the MCS software and load the desired print file. 
* Check the build time and layer number to see that the build processor has correctly interpreted the desired 3D print model. Once satisfied, make sure that the “Reset” button has been pressed and click “Start Process” button. The Setup Build Job window will appear. Select the desire initial layer and Initial Exposure. It is advised to use Initial Exposure for the first few layers to increase penetration with the substrate. After that, press “Start Build Job” button.
* The build process begins and is carried out automatically.
* During the first 15 layers is important to observe whether the process is running smoothly. Things to observe:
1. Is the powder being deposited equally while the recoater is moving forwards and backwards? If not, the blade switch mechanism behind the process chamber door may be raised and needs to be lowered.
* In case of any issues, it is possible to pause the process between the layers and open the process chamber when it is safe to do so. After remediating the issue, the process chamber door and cover barrier can be closed, the reset button pressed, and the process started again.
* If an intervention in the process is required (i.e., opening the process chamber), technical staff must wear appropriate PPE which include powered air-purifying respirator (EN166 and FFP3 EN149), single use nitrile gloves (EN374), anti-static coveralls (EN1149-5).

## Cleaning Up the Process Chamber

* After the build process is finished, the remaining metal powder in the process chamber needs to be dispensed into the two conversion shafts and the process chamber completed cleaned.
* Technical staff cleaning the process chamber must wear appropriate PPE which include powered air-purifying respirator (EN166 and FFP3 EN149), single use nitrile gloves (EN374), anti-static coveralls (EN1149-5) and safety shoes with steel/composite toe caps (EN20345).
* Before opening the process chamber ensure that the temperature of the build plate has cooled down to below 50 ºC and oxygen level is above 18 % by checking the sensors status in the MCS software.
* Follow procedure to open the process chamber and vacuum the condensate powder that accumulates on the inner sides of the process chamber. With the door open, insert the spatula and brush tools provided by SLM (non-sparking tools) inside the chamber.
* Close the chamber door and cover barrier, press the reset button, and flood the chamber with inert gas (Manual control → Flood Inlet/Outlet “Open”). After oxygen level is below 0.5%, close the Flood Inlet valve to reduce the pressure in the chamber.
* Raise the platform by about 20 mm, open the cover barrier and insert the access gloves to start pushing the remainder powder into the conversion shafts. After cleaning the remaining powder, raise the platform by about 20 mm again and continue this until almost all the powder from the chamber is removed.
* Then, open the chamber and vacuum up any remaining powder. Pay attention to vacuum the bolts and inner parts (e.g., recoater blade) which can accumulate powder.
* The process chamber can only be wiped down with IPA once the temperature in the build platform is below 30 ºC, the build plate has been removed from the chamber and the interior of the process chamber is cleared of excess powder using the AMC 330 industrial vacuum cleaner.
* Clean the beam entry glass using the approved IPA spray bottle and cleaning cloth. Follow the procedure in the SLM manual (pg. 136).

## Handling and Filling Metal Powder into Hoppers

* Technical staff handling metal powder must wear appropriate PPE. This includes powered air-purifying respirator (EN166 and FFP3 EN149), single use nitrile gloves (EN374), anti-static coveralls (EN1149-5) and safety shoes with steel/composite toe caps (EN20345).
* Use of a platform ladder is required for filling metal powder into hoppers as it provides good foot support for technical staff holding the powder bottle.
* Care must be taken to manipulate powder slowly, to prevent the formation of a dust cloud.
* Heat sources, water, oxidizers, acids, and alkalis should be avoided in the presence of powder.
* Powder should only be manipulated with non-sparking tools and equipment.
* For filling the hoppers, start by removing the empty metal powder bottle from the main tank. Use the platform ladder to reach the main tank and close the check valves from the empty powder bottles. Release and remove the clamp fastener, remove the powder bottle, and set it on the floor.
* When filling metal powder into hoppers, make sure that the centering ring is correctly placed on the connection nozzle. With the closed check valve, place the powder bottle filled with metal powder on the connection nozzle and secure with the clamp fastener. Open the check valve at the connection nozzle and powder bottle and let the powder run into the main tank.
* Determine whether the powder bottle is completely empty trough acoustic checks (tapping on the powder bottle).
* Close the check valve on the powder bottle and connection nozzle and remove the empty powder bottle and place it on the floor. Place a cover with a centering ring on each opening of the connection nozzles and secure each one with a clamp fastener.

## Sieving the Metal Powder with the PSM 100

* The sieving process is used to recover used metal powder, so that rough powders reminiscent from the build process (e.g., condensates and non-melted particles) are removed accordingly.
* Technical staff sieving the metal powder with the PSM 100 machine must wear appropriate PPE which include powered air-purifying respirator (EN166 and FFP3 EN149), single use nitrile gloves (EN374), anti-static coveralls (EN1149-5) and safety shoes with steel/composite toe caps (EN20345).
* To start, first check whether the oversize grain bottle (small bottle) is empty by tapping it with any metallic tool. If the bottle is empty a distinctive sound can be heard. If it is full, then the powder needs to be disposed of in the waste drum located behind the SLM machine.
* Now install the usable grain bottle on the bottle holder beneath the valve using a sealing ring. Raise the bottle holder and secure the usable grain bottle on the reducer with a clamp closure. After installing it, open the check valve so that the lever is pointing to the flow direction.
* Remove the cover on the connection port of the powder supply and install the used powder bottle using the pivoting arm. Make sure that the check valve is closed while performing this operation and do not open it after installing the bottle.
* Turn the machine ON using the lateral switch and press the reset button, the oxygen measurement unit will start. Wait 1-2 min until the unit has heated up and check that the oxygen measurement is correctly calibrated: display at approx. 21%.
* Flooding is performed to remove the oxygen from the sieving pipes.  Before this, it is very important that the check valve of the upper used bottle is closed, otherwise powder will enter the filter unit during flooding. To activate flooding, turn on the “POWDER OUTLET” switch, followed by the “POWDER INLET” switch and finally the “FLOODING” switch. The oxygen value will now reduce. Wait until it is below 0.5%.
* After the oxygen level is below 0.5%, the “FLOODING” switch can be turned off. Next, activate the “SIEVING” switch and open the manual valve on the supply powder bottle. The powder will start to be sieved and separated into the oversize and usable grain bottle on the bottom.
* Wait 3-5 min and using a metallic tool, start tapping the supply powder bottle to check if it is empty. Once it is empty, the “POWDER INLET” switch can be turned off again and the manual valve on the supply powder bottle can be closed. Wait a few minutes until there is no longer any metal powder in the feed port. Tap the usable grain bottle on the bottom to check that it is full. Switch off the “SIEVING” and the “Powder OUTLET” switch.
* The manual valve of the supply powder bottle can now be closed (the leaver is at a 90-degree angle to the flow direction). Tap on the connections with a soft-face hammer to ensure all the powder is removed from the connection. Remove the clamp closure and place the bottle on the floor.
* Use the full bottle to refill the machine into the hoppers (Handling and Filling Metal Powder into Hoppers).
* After this, reinstall the empty powder bottle in the conversion shaft and ensure that the leaver is pointing to the flow direction.
* Cover and clamp all connections, and tun off the oxygen measurement unit and main switch.

## Build plate and Part Removal
* After completion of a build, parts must be removed from the build plate.
* When removing parts from the build chamber, technical staff must wear appropriate PPE. This includes powered air-purifying respirator (EN166 and FFP3 EN149), single use nitrile gloves (EN374), anti-static coveralls (EN1149-5) and safety shoes with steel/composite toe caps (EN20345).
* Once released from the build platform, supporting material typically must be removed from the fabricated parts using a variety of hand finishing operations, typically involving specialist tools with non-static properties. Protective gloves (EN388) should be worn as needed during these hand finishing operations.
* The build plates must be mounted securely to a metal table before removal is attempted.
* Any metal powder that was entrained in the supporting material must be cleaned up with AMC 330 industrial vacuum cleaner.
* The used build platforms must be machined flat for future reuse for new parts. Suitable grinding operations are available as a service from UoM Workshops, which will be charged to appropriate project code if required.

## Use, Storage and Care of PPE
* The batteries for the powered air-purifying respirator (PAPR) units shall remain plugged in to the chargers when not in use.
* Full-face respirators are to be cleaned with blue paper rolls embedded in isopropyl alcohol (IPA) on a regular basis to remove any accumulations or potential respiratory hazards (e.g., metal powder). Cleaned respirators shall be stored in individual sealed (ziplock-type) plastic bags to keep them ready for the next use.
* The PAPR units, protective gloves and clothing are to be stored in the designated PPE cabinet within the SLM zone. Specifically, these items are not to be removed from the SLM zone so that any trace amounts of metal powder are contained and not spread to other areas unintentionally.
* The disposable coveralls need to be replaced often (once a week) depending on the use and need to be checked before each use for tear/wear, in which case a new coverall need to be used.

## Use and Checking of House Gases
* Technical staff must be familiar with safe use of compressed gases.
* The SLM system uses Nitrogen or Argon gases depending on the powder material being used to provide an inert atmosphere in the build chamber and compressed air for the optical bench.
* The SLM system includes built-in oxygen sensors to monitor the system environment (both within the build chamber and in the machine cabinet), as well as a visible/audible warning system to warn of potential hazardous situations. As an extra precaution, two additional oxygen sensors and alarm system are installed in the laboratory within 5 m from the machine to monitor the oxygen concentration in the SLM area.

## Cleaning Up Spilled Metal Powder
* Technical staff cleaning up spilled metal powders must wear appropriate PPE. This includes powered air-purifying respirator (EN166 and FFP3 EN149), single use nitrile gloves (EN374) and anti-static coveralls (EN1149-5).
* Remove all sources of ignition, ventilate area of spill, and avoid contact with water.
* Display a clear and visible sign to warn other users about possible contamination and cordon off the spill area.
* Clean up spills in a manner that does not disperse dust into the air, using non-sparking tools only.
* Recovered bulk powder should be placed into original vendor-supplied storage container.
* Remaining non-recoverable powder should be vacuumed up using AMC 330 industrial vacuum cleaner.

## Disposal of Metal Powder and Cleaning of SLM zone
* Technical staff disposing metal powder and cleaning the SLM zone after each use must wear appropriate PPE. This includes powered air-purifying respirator (EN166 and FFP3 EN149), single use nitrile gloves (EN374) and anti-static coveralls (EN1149-5).
* Any powder remnants that cannot be reclaimed for reuse should be vacuumed up with the SLM vacuum cleaner.
* When full, the vacuum cleaner should be emptied according to the maintenance instructions in the SLM accessories manual.
* The resulting metal powder sludge from the cleaned SLM vacuum cleaner should be stored in the designated metal drum container.
* Any PPE and blue rolls used for cleaning the SLM zone are to be disposed in the designated “Hazardous Bin” adjacent to the SLM machine. This waste is to be double-bagged and when the bin is full, the bags must be moved into the second metal drum container.
* The waste drums are to be always kept in demarked location behind the SLM machine.
* When the drums are 2/3 full, WasteCare will then be contacted, and the drums will be moved to the loading bay only on the collection day.
* The waste drums and bins in the SLM zone are to be kept always closed to avoid contamination in the Heavy-Duty lab.
* The external surfaces of the SLM machine (below the process chamber), bench tops and ESD matts are to be cleaned with blue rolls wetted in isopropyl alcohol (IPA) every time after use.

## Emergency Response for Fire Involving Metal Powder
* In case of fire or ignition of metal powder, first get yourself and all nearby personnel out of the danger area. Then activate the nearest fire alarm (located near the fire exit door) and contact Security Lodge by calling 0161 306 9966 from a phone outside the danger area. Leave the building using the nearest safe exit and assemble at designated meeting point: outside the Greenhouse Café.
* For extinguisher-trained personnel only:
  - Activate the nearest fire alarm (located in the hallway) or call 0161 306 9966 before using the extinguisher.
  - If the fire is small, use ONLY Class D extinguisher in an attempt to put the fire out.
  - Use only ONE extinguisher, and then leave the building using the nearest safe exit.
* Important Safety Note: Use only Class D fire extinguishers for fires involving metal powder. Do not use water due to the reactivity of the metal powder with water.

## Emergency Shutdown of SLM system
* In case of emergency, press the red Emergency Stop button on the right side of the process chamber door to stop the SLM 280 system immediately. Pressing this will stop movement of components and the unit will be disconnected.
* After this, turn off power at the main switches behind the machine if safe to do so.
* Emergency situations that would require an emergency shutdown of the SLM system may include fire evacuations or fire of one or more system safety controls.
* When restarting the machine after emergency shutdown, ensure no dangerous conditions prevail:
  - Check the emergency stop button by rotating in the direction of the arrow and pulling.
  - Acknowledge the fault messages in the control software using the touch screen control.
  - Press the Reset button.

## Normal Shutdown of SLM system

* After completion of a build, removal of the parts, and cleaning of the build chamber to prepare for the next build, the system can be powered down by (1) ending the MCS control program, (2) shutting down the control computer, and (3) turning off the machine main switch. After shutting off the machine main switch, watch for the three lights above the cabinet to flash red indicating complete shutdown.
* If the machine is expected to be used twice in the same week, then it does not need to be turned off.

Maintenance of SLM system and accessories
* The SLM system and its accessories must be maintained according to the instructions in the SLM operations and accessories manual. Specific guidance is provided for maintaining the chiller unit, the recirculation system, the vacuum cleaner, and the recoating blade.
* A maintenance schedule has been created which must be kept up-to-date and all maintenance activities recorded in the logbook kept by the machine.
* Technical staff should never attempt to modify, fix, or maintain the SLM laser system or to access the laser delivery path. Laser covers and laser safety controls are to remain intact for all SLM operations. All maintenance of the laser system is to be performed by a trained SLM service technician during service visits arranged yearly or when necessary. A laser safety warning sign is to be placed at the entrance to the laboratory when the SLM service technician is working on the laser system.
* Appropriate PPE must be worn when replacing the recoater blade. This includes powered air-purifying respirator (EN166 and FFP3 EN149), single use nitrile gloves (EN374) and anti-static coveralls (EN1149-5). Prior to removing the recoater, switch off the power amplifier in the control menu.
* Important Safety Note: Replacing the dirty filters to maintain the recirculation system is viewed as potentially the most hazardous operation necessary in using the SLM system. The recirculation system holds two large filters on the side of the machine that filter the inert gas flow and collect fine metal condensate from the build chamber. Each of the filters is grounded to the cabinet of the recirculation system to reduce the change for static discharge. The PPE for this activity consists of air-purifying respirator (EN166 and FFP3 EN149), single use nitrile gloves (EN374) and anti-static coveralls (EN1149-5). The filter change must be performed according to the instructions in the SLM manual (pg. 223-239).  Once a filter is removed, the filter should be wetted with water in the filter rising unit to further prevent static discharge and the dampened filter must be placed submerged in the waste drum – the filter cannot be reused or stored.

## Equipment cleaning and maintenance for powder changeover
* If the SLM 280 is going to be used for multiple materials, extensive cleaning/maintenance work must be performed for each material change.
* Cleaning the system for a change of material should take place from top (main tank) to bottom (powder bottles). This is to avoid contamination of components that have already been cleaned.
* Cleaning can be only carried out with isopropanol only.
* Starting by disassembling the recoater, placing it on the work bench. Then, move the recoater holder back to the fill position, otherwise the loader cannot transport any metal powder.
* Place the discharge shaft under the filling shaft inside the process chamber. The discharge shaft must be pushed under the filling shaft to the stop, so that the valve of the filling shaft opens, and the metal powder can fall through the discharge shaft into the back conversion shaft.
* Close the process chamber and press the reset button. Then, empty the main tank by entering the value 500 in the input field under the [Powder Loader] item. Repeat the steps until the fill level indicators of the main tank indicate that the main tank is empty and replace the powder bottles in the back conversion shaft when they are full.
* Using the platform ladder, remove the ceiling covers. Remove the 4 powder sensors and argon pipe from the main tank. Unclamp and unscrew the main tank and remove it, put it in the work bench. Clean the rail of the mail tank.
* After that, remove the voltage and encoder cables (yellow and green) from the powder loader and disassemble it via three screws. Two are hidden in the top part and another one is one on the side.  Then remove the 8 lateral screws from the powder loader. Place the powder loader on the work bench. It will need to be disassembled, cleaned with IPA and reassembled.
* Remove the two conversion shaft tanks by removing the top clamp closures and the main M6 screw holding the tank in position.
* Remove the sieve of the conversion shafts by removing the fastening screws (6 in total) and disconnecting the powder sensor.
* Inside the process chamber, remove the left side inner wall and the bottom gas outlet (black component), then remove the bottom right side gas inlet. It may be necessary to loosen the screws near the door chamber to be able to remove the right gas inlet.
* Remove the screws of the build platform frame and the two mesh filters of the conversion shaft. Also remove the round cord underneath the frame and place it on the workbench.
* All the removable parts should be on the workbench now. It will be needed to wipe down all the parts with IPA, inclusive the interior of the recoater, which needs to be disassembled, cleaned, and reassembled.
* Wipe down the process chamber with IPA and vacuum cleaner if necessary.
* Close the process chamber and press the reset button. Move the platform to the bottom and wipe down with IPA the walls of the build envelope. Squirt IPA through all the wall and then move the platform to the top and bottom again, until there is no more powder in the walls and on the platform seals.
* Once the process chamber has been cleaned, reinstall the removable parts in the process chamber, the conversion shafts, powder loader and the main tank. This step should be done in the reverse order from the disassembly.
* Follow SLM.SOP.6 to refill the hoppers with new powder.