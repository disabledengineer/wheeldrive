# wheeldrive
Innovative custom wheelchair drive which utilizes high power BLDC motors.

I talk alot about this project on my Instagram!  
https://www.instagram.com/crazey96/

![](https://github.com/crazey96/wheeldrive/blob/master/images/overview.jpg)

## Motors
In general BLDC motors are the best choice for this application because they offer high torque and power while being low weight. I decided to go with 6374 Sensored Outrunner Motors. Usually they can be operated with up so 13S (~54V) and 50A. That's up to 2.5kW power per Motor (5kW in total) while being low weight (one motor weighs ~800g). Furthermore the KV rating is very important because it determines how much torque and top speed you want to have. The lower the KV, the lower the maximum RPM, but the higher the torque. I recommend going with somewhere between 30KV-60KV. Here are some good examples:  
https://alienpowersystem.com/shop/brushless-motors/aps-6374s-sensored-outrunner-brushless-motor-30kv-2800w/
https://alienpowersystem.com/shop/brushless-motors/aps-6374s-sensored-outrunner-brushless-motor-60kv-2800w/
## Motor Controller
I recommend using the VESC because it's an open-source project and can be programmed specifically for this application. Many ESCs are designed for RC-Cars, Airplanes, or boats. Using a VESC you have a wide range of settings to perfectly fit your needs. There are many tutorials on the internet on how to set this up, so I won't go into detail. However here are some tips:
+ Use FOC for more start up torque
+ Start with low motor amperage (10A, then go up to 20A or even 50A)
+ Make sure your battery amperage is set to half of what your battery is rated for!
+ Use current control, that way you control the torque instead of the RPM
https://vesc-project.com/
## Mechanics
I used HTD5M Timing belts to transfer the torque from the motor to the wheels. The belts must be at least 9mm wide to properly transfer the torque without skipping and damaging the belts and pulleys. To properly tension the belt I simply used two bearings as a idler pulley, there is a cutout for it on the motor mount!
