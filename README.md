# Casper
Converting a telescope into one that automatically positions itself to view planets and other celestial bodies based on user input.
2 Stepper motor axis will position its azimuth, basically cardinal direction, and altitude, the angle between the horizon and straight up. To find the target a camera on the telescope tube will take pictures of the sky and use plate solving, which is where the position of the stars in the sky are compared to a database of known stars to find the coordinates of where in the sky the telescope is pointing. A Raspberry Pi will handle the bulk of the computing while a microcontroller drives the stepper motors. A belt system will be used to gain gear reduction between the stepper motors and the load shaft.
This project is split into 3 parts, mechanical, electrical, and software. On the electrical side I am making a custom PCB controller for the telescope. This includes a STM32 microcontroller, Raspberry Pi 0 2W, stepper motor drivers, power regulators, and all other supporting hardware.
The mechanical part will be designing a mechanical drive system for both axes out of commercially available parts and custom 3D printed parts.
On the software side, the Raspberry Pi will run the plate solving software and tell the microcontroller how much to move each motor. The Pi will also host an interface where user commands can be sent to operate the telescope.



