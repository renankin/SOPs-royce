# SOPs for the welding cell

## General Safety Concepts

* Only qualified personnel are authorized to operate the Welding Cell. Qualified personnel are those that have been instructed by the technical staff in charge of the Welding Cell.
* All required training must be completed before being considered qualified to operate the Welding Cell.
* Technical staff must observe and follow the safety warnings posted in the laboratory and provided in the manuals and other safety documentation. 
* Technical staff must wear the required protective equipment, and risk assess the activity before carrying out any work.
* The welding cell has an interlock system designed to be able to operate in AUTO mode only when all personnel are outside of the enclosure. Users must not disable or override the built-in safety features of the system. The Enclosure is fitted with E-stops which will cut power to the robots and welders in the event of an emergency or mal function. All users are to be aware of the location of E-stops.
* The robots are configured with SafeOperation interface – this applies a software stop to both TEACH and AUTO mode. This prevents the robots moving outside the work area and has the same effect as a mechanical end stop applied to the robot axis. The users are not allowed to change the Interface as especial training is required for this.
* Flammable materials and sources of ignition should not be stored in the working area inside the Welding.
* Working with metal powder requires several safety precautions, including respiratory protection, protective gloves, non-sparking tools and equipment, anti-static grounding, and careful manipulation to prevent dust clouds. See specific procedures below for working with metal powders.

## Switch on the system

* To turn ON the robotic cell, the user should first turn on the welding power sources:
 - 2 CMT units;
 - 2 TransTig Units;
 - 1 Plasma Module;
* Then the user should turn ON both robot controllers simultaneously. To do this, open the key locker using the passcode provided and collect the two yellow keys (Nr. 16 and 17). Open the padlocks that are on the controllers which are found on the back of the welding cell. Then switch ON both controllers.
* After both robots are powered up, the HMIEasy screen needs to be selected in both smartPADs. To do this, click the Robot button -> Display -> “HMIEasy”. Then, press “Emergency Stop Reset” on the control panel to reset the welding equipment.

## Operation of the enclosure

* The robots are designed and interlocked to only perform welding in AUTO mode when the users are outside the enclosure and the interlock master key is inserted in the safety panel.
* The operator with the master key is responsible for ensuring that no other users are inside the welding enclosure and interlocks are active. However, for robot programming and verification and loading/unloading the workpiece or preparing for the welding task, the user is allowed inside the cell. During these operations, the user can carry out robot movement using TEACH mode whilst observing the control measures detailed below.
* To access the master key, both access doors need to be closed and the master key removed from the safelock.
* Turn the main switch for the machine to the “ON” position.

## Operation of the robots

* Both controllers should be turned ON at the same time.
* Prior to being able to run welding programs, the user needs to carry out Master Reference and Brake Test. This is to determine the position of the robot in the cell and to verify if the axis brakes are operational.

## Operation of the welding equipment

* The power sources are connected to the robot controller trough a digital interface, called DeviceNET. 
* To operate the welders, the user needs to turn on the shielding gas, which will be used to protect the melt pool during welding.
* Ensure a good connection of ground cables with the welding table. The clamps should be placed closest to area to be welded as possible. Ensure that the ground is not clamped on a rusty surface, but rather on a clean metal surface.
* The welders are connected via DeviceNet with the robots. These exchange I/O signals to enable automatic welding. Example of signals are: “Weld Ready”, .. Some of these are input signals while others are output signals.
* To use the welders, they need first to be switched ON after the robots are turned ON. The shielding gas must be appropriately connected. For the plasma unit, Argon is used for shielding gas and for pilot gas.
* The ground cables need to be connected to the correct terminal to close the welding circuit. When using the GMAW process, the ground cable is connected on the negative, for the PAW process, it goes on the positive.
* The welding parameters, i.e. current, voltage, wire feed speed, etc. are defined and saved in a Job file inside the power source. The robot then calls the Job file when doing a welding seam, which applies the saved settings for the specific seam.
* When using welding wires, the correct liners and wire diameter needs to be considered. When changing the wire diameter, the wire feed rollers need to be replaced.
 - Steel and its alloys => bronze liners.
 - Hard alloys such as Ni-based alloys, Ni-Cu, etc. => graphite liners.
 - Soft alloys => graphite liners.


