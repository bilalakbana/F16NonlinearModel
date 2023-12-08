# F-16 simulator model for real-time joystick-piloted simulation 

The f-16 simulator model is developed in Simulink encompassing Aerodynamics, Propulsion, Actuator, Mass, Kinematics, Environment, and visualization - FlightGear - blocks. 

A joystick device can be connected to the model to control the aircraft and project the attitudes and positions on FlightGear. 

A short video on simulation is shared in:  
https://www.youtube.com/watch?v=vfG6OFAr69o

Model data is obtained from NASA TP 1538, which includes nearly 50 aerodynamic tables, and thrust values based on the throttle input, Mach number, and height.

Controller inputs are:  
δa    ->    ailerons                   -> [-21.5,21.5] deg  
δh    ->    elevator                   -> [-25, 25]    deg  
δr    ->    rudder                     -> [-30, 30]    deg  
δsb   ->    speed brake                -> [0,60]       deg  
δth   ->    throttle                   -> [0,1]         -  
δlef  ->    leading edge flap angle    -> [0,25]       deg  
  
Aircraft states are:  
[u v w]           ->  body velocities        ->      m/s  
[phi theta psi]   ->  euler angles    ->             rad  
[p q r]            -> angular rates    ->            rad/s  
[xe ye ze]        ->  north-east-down positions  ->  m  
Pa             ->     actual power      ->           percentage  
  
Reference:  
Simulator study of stall/post-stall characteristics of a fighter  
airplane with relaxed longitudinal static stability, NASA-TP-1538  
  
To access the model contact via:  
simulatortechs@gmail.com
