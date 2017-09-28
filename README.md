# clearpath-sc-single

A cut down board with similar electronics to the Clearpath SC4-Hub, but designed for single motor use.

![Iso Render](renders/iso.png?raw=true "SC Single Render Iso View")

## Overview

The Clearpath line of CNC servo motors from Teknic are great for robotics due to tight integration of controller and motor.

![Clearpath Motor](renders/clearpath.png?raw=true "Clearpath Motor")
![SC4 Hub](renders/sc4.png?raw=true "Teknic's SC4 Hub")

The SC series are software controllable, but rely on the use of a communications hub for level shifting and e-stop etc. This hub is designed to handle 4 motors and daisy chaining, and offers outputs to control brake solenoids and e-stop switches.

My application is space constrained and has no brake, so this single channel board offers the same main functionality (but we lose e-stop and brake outputs, and less defensive filtering on power input) in a reduced form factor. The serial input and USB functionality is maintained, and all OEM level hardening/filtering on communication lines on the SC4 is maintained. 

![Top Render](renders/top.png?raw=true "SC Single Render Top View")

12-24V input power to provide signal level power. USB to serial is powered from the USB host. Header supports other TTL level serial devices if desired.
