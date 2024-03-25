# SOPs for Micro Electron Beam Welder

## General Use of MEBW system 
* Prior to start using the instrument, check that the instrument has no sign of wears or damage and check that the gas valve at the back is showing about 6 bars.
* Open the padlock and turn on the instrument using the main switch. Press the green start button and log in on the remote-control panel (RCP). PIN is "123456".
* Turn on the supporting PC and log on windows. User is "focus" and password "focus". On the desktop, open the "FOCUS Loader" software. Log in as "supervisor" with password "focus". The current role should change from "Operator" to "Supervisor".
* Press "Start Mach4 (CNC)" and "Start DacPath". Two additional windows will open.
* Hold "VENT CHAMBER" to open the chamber door. Look inside the chamber and check there is no damage inside the camera before starting to load your samples. If there is, report immediately to the responsible technical staff.
* Use the HyFlex white gloves provided to load your samples inside the chamber. Make sure that the sample is properly secured to the welding fixture.
* Close the process chamber and hold the green start button to turn on vacuum (If the chamber is already under vacuum the user needs to press "PUMPING ON/OFF" to start vacuum). It takes about 4 min to complete vacuum, and a distinctive sound will come up after the electron beam gun goes down below 4 x 10-4 mbar.
* On Mach4 software, press "Enable" to activate the remote CNC controller. Press "JOG" and move the stage by pressing "X", "Y" or "ROT" and using the jogging wheel. Turn on "CHAMBER LIGHT" on the teaching pendant and move the sample below the electron beam column.
* To turn ON the beam, press "HIGH VOLTAGE" (some noise may occur as the electrode stabilises). The high voltage can be adjusted by opening the front panel below the process chamber and adjusting the high voltage knob. After that, press "FILAMENT HEATING" on the teaching pendant. Press Scan&View (TV off) twice to turn the TV mode on. Adjust the beam current to about 0.2 mA (low currents avoid damaging the surface of the sample).
* Try to adjust FOCUS and observe if the image is static while doing this. If not, try adjusting the stigmator. This setting can be accessed via "Beam ctrl" tab on the second menu. Press "Stigmator" and adjust it using the two middle bottom knobs. Increase the zoom level for a finer adjustment

## How to do a linear weld
* For positioning the electron beam relative to the weld seam, use the on-screen cursor. The beam centre needs to be adjusted first. Choose the zoom level required and move the stage to a position on the plate that will not be used for welding. Turn off TV mode and press "Beam current" twice and leave it ON for 1-2 sec using 0.50 mA. This will create a small hole in the plate. Turn on TV mode again and use that point to adjust the center of the on-screen cursor relative to the weld spot created. The cursor can be adjusted on Menu 2 of the Scan&View mode. Click "Cursors" once and adjust using the bottom middle knobs. The position of the beam is now calibrated relative to the centre of the cursor.
* Go to Mach4 interface and press "Load G Code". Go to "Documents/Standard Programs/001_linear_weld_ramp.tap" and click confirm.
* Edit the program with your process variables and desired position.
* To define the position to be welded, jog the stage to the beginning of the weld seam and reset the axis (X=0, Y=0, Z=0) using the TV mode ON. Then move to the end of the seam and annotate the new position. Click "Edit G code" and update the program with the coordinates. Define the positions mid-length to include ramp-up and ramp-down slopes. This is to avoid creating a unstable melt pool at a high power at the beginning of the weld.
* After choosing the desired beam current the user must look at PDF "Focus-Beam-Filament" located on Desktop to find out the focus offset and filament current required during welding.
* After this, save the file in the "Documents/Users/YourName" folder and close it. The first test should be with "Simulate on" to check if the program is running ok. Press "Start" to run the program. If everything is ok, then disable "Simulate on" to start the actual weld.
* If you wish to make a pause during your work, it is ok to turn off the "FILAMENT HEATING" to avoid degradation of the electrode.
* To remove the specimen, turn off "FILAMENT HEATING" and "HIGH VOLTAGE" on the teaching pendant and hold vent chamber. Before opening the process chamber, make sure to DISABLE the CNC controller. Use the provided heat-proof to remove the specimens and place it on the heat-proof alumina plate. Make sure there is a sign "Caution hot surface" next to the sample to avoid any other users touching the hot sample.
* Close the process chamber and turn on the vacuum by pressing the green start button. Wait a few seconds and proceed with shutdown procedure.
* The shutdown involves pressing the emergency stop button, shutting down the supporting computer and finally the main switch. Use the padlock to protect anyone using the system and put the key inside the right drawer. Do not forget to release the emergency stop button afterwards.

## Installing the CNC Rotary Table
* Prior installing the CNC rotary table is necessary to turn off the manipulator control by opening the right cabinet door and switching off the main switch.
* After doing this the CNC rotary table can be fixed to the X/Y stage and the connector plugged into the socket found on the right-hand side of the X/Y stage. There is a cover protecting the plug. The red circle on the connector of the CNC rotary table must be facing the user before installation.
* After plugging the connector and properly fixing the CNC rotary table to the X/Y stage, the manipulator control main switch can be turned on again.

## Replacing the cathode
* On the teaching pendant, go to "Preparation tab" on the Menu 2/2 and hold "Vent both", to stop vacuum in the workpiece chamber and the EB generator.
* Turn off the whole MEBW-60 system using the emergency off switch. Wait for approx. 30 seconds until the safety lock mechanism allows the opening of the EB generator. This can be verified by observing if the "LOCK" led light is off on the yellow pump gate.
* Open the four cap head screws using a suitable Allen key (nr. 5). The fours screw can be found inside a bronze bush. Loose the screws and leave the inside.
* Carefully pull the handle upwards using two hands. When the cathode is fully raised, the safety lock engages automatically and is safely fixed in the upper position. Ensure that the cathode is secured and cannot fall.
* Before removing the cathode, touch the cathode casing with the discharge head (to remove any static charging) and place it back to its holder.
* Using the heat-proof gloves (be careful the cathode can be hot!), turn the cathode clockwise by hand while pushing it slightly backwards to release the bayonet lock. Take care to protect the cathode from falling. Place the cathode on the heat-proof surface beside the process chamber.
* The cathode case should be closed again after removing the cathode to prevent contamination of the cathode chamber. Release the safety lock mechanism and carefully lower down the cathode chamber.
* The tungsten filament can now be replaced. Use a nitrile glove for doing this procedure and ensure that the cathode is at a safe temperature before touching it.
* Screw out the two Allen screws on the upper part of the cathode holder and remove the upper case.
* Loosen the two Allen screws of the filament brackets and remove the filament with a tweezer.
* Carefully insert the new filament into the clamps until it makes contact to the bottom. Then close the clamps while tightening the screws. After the assembly, check that the filament is centered in the holder.
* Place the top part on the bottom part matching the "X" mark on both parts. Take care not to move or damage the filament in this step.
* The filament must now be aligned in the center of the cathode holder. For this purpose, there is a pair of screws opposite each other in both the X and Y direction. By loosening one set screw, the filament can be pushed in the opposing direction of that screw. It is necessary to release the screw in one side and screw the other side as the filament can be only moved by a push. Only apply a small force to not damage the cathode holder. A microscope is provided that can help with the centering. After adjusting all the screws should be slightly firm to hold the filament in position.
* Now the height of the filament is adjusted. For this, the height tool is placed on the aperture of the cathode holder. The centering pins of the height tool are inserted into the two holes provided for this in the aperture. The height is adjusted by rotating the height tool. Turning the gauge clockwise means the filament is pushing further out of the aperture. The movable inner cylinder of the height tool should be flush with the surrounding case (black plastic).
* After this the cathode holder can be installed again into the cathode case.
* Raise the cathode case again and secure it with the safety lock mechanism. 
* Slide the two slots of the bayonet on the cathode over the bayonet pins of the holder. Watch for the correct orientation - the "X" mark should be facing you. 
* Fit the cathode holder into the bayonet slot, press it firmly and then turn it counterclockwise until the cathode holder is fully engaged.
* Release the self-locking mechanism whilst holding the leaver-bar and carefully lower the cathode chamber.
* Screw the four cap head screws hidden inside the bronze bush. 
* The procedure is complete and now the beam centering must be carried out.

## Centering the beam
When using low beam currents (up to 15 mA), centering can be carried out with "Wobble" procedure, otherwise the "Anode current" procedure must be done.
“Wobble” procedure:
* In the Wobble procedure, the user must first vent the process chamber and install the focus adjustment tool inside the chamber. The adjustment tool can be installed on the X/Y stage (using the T-slot plate) or it can also be fixed to the rotary CNC unit if this is adjusted to an angle of 180º.
* The TV mode needs to be turned on and an electron image should appear in the screen following the procedure described in SOP "Using the instrument".
* Jog the X/Y stage so that the holes on the adjustment tool are in the middle of the screen. Try adjusting focus the best you can. 
* On the RCP go to "Beam ctrl" and check that the electromagnetic "Centering" is switched on and that the X/Y axis are set to 0%.
* Then long press Focus to activate Wobble. This will cause an image shift depending on the current focus setting.
* To start the procedure, first loosen the 4 set screws hidden inside the bronze bush (Allen key n.5).
* The aim is to reduce/eliminate the image shift by using two sets of screws located in the top of the cathode chamber (near the high voltage cable). By loosening a set screw, the inner part of the cathode can be moved in the respective axis direction with the opposite set screw. The movement can only be performed by pushing (not pulling). Only a small force may be applied to the set screw, otherwise there is a risk of damage.
* Observe the SEM monitor image during adjustment to determine the point of least image shift. IF the image shift increases again, the cathode insulator needs to be moved in the opposite with the opposite screw. Repeat the process alternately on both axes until the desired centering quality is achieved (minimum or no image shift).
* After this, tighten all four screws that are inside the brozen bush carefully and with litte force and the four screws used to adjust the beam centering. While doing so, oberve the SEM image on the monitor; the image must not shift again.
* Switch off the focus wobble. To check the procedure was successful, defocus the beam manually on the Focus knob on the RCP by changing the focus current. The SEM image on the monitor must not shift.

“Anode current” procedure:
* For this, using the TV mode, go to "Preparation" tab and press filament once and then reduce the filament heating current to 3.2 A.
* Increase beam current to approx. 1 mA.
* To be continued.
