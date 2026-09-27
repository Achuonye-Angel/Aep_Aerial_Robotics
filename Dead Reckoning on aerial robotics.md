# Dead Reckoning

### What is dead reckoning?

##### Dead reckoning is the process of estimating the location of a device using the previous location and the determined speed.



#### In the case of aerial robotics:

Dead reckoning in aerial robotics is the process of estimating an aircraft's current three-dimensional position, velocity, and attitude by continuously propagating a known initial state using onboard measurements of linear acceleration and angular velocity. Unlike ground vehicles that rely on wheel encoders, aerial dead reckoning integrates high-rate data from an Inertial Measurement Unit (IMU) through kinematic equations, rendering it highly susceptible to time-dependent error accumulation (sensor drift) in the absence of external absolute references.



### Types Of Dead Reckoning 

There are various types of dead reckoning. They include;

1. Inertial Navigation System (INS): This uses the Inertial Measurement Unit(IMU) consisting of accelerometers and gyroscopes. It integrates 3D acceleration and angular velocity over time to calculate velocity and position. It is mainly used in drones, submarines and aerospace. It suffers from severe mathematical drift over time.
2. Doppler Dead Reckoning: This uses a sensor known as Doppler Velocity Log(DVL) to bounce sound waves off the sea floor or surrounding water. It measures the shift in the returning echoes to measure the vehicle's exact speed. It is mainly used in under water robotics(AUVs and ROV's).
3. Pedestrian Dead Reckoning(PDR): It is used as wearables such as smart watches, smart phones. It uses a compass for direction and a step counting algorithm to estimate step length.
4. Visual Odometry(VO): It tracks how distinctive pixels or features move across sequential camera frames to measure how fast and in what direction it is going.
5. Wheel and Track Odometry: This measures the physical rotation of a robot's wheel or tracks using rotary encoders. Knowing the wheel's diameter and rotation speed allows the system to calculate the distance and angular speed.



### How Does Dead Reckoning Work?

Dead reckoning works by in following three distinct steps, which are:

* Establishing a starting point
* Measuring the motion of a system using internal sensors
* Calculating the new position: New Position = Previous Position + (Speed x Time) along the Heading angle.

