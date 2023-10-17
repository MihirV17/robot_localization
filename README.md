# Robot_Localization Project
### By Kenta Terasaki and Mihir Vemuri

## Particle Filter Description

In the context of our robot localization, we have developed a comprehensive architecture for implementing a particle filter. This particle filter aims to solve the problem of localizing a robot within a given map by leveraging information from both lidar and odometry readings. The primary objective is to provide a reliable pose estimation that can subsequently be utilized in various applications, such as path planning algorithms or similar processes. While our current implementation is still a work in progress and not performing as expected, all the individual components of the particle filter have been meticulously put in place. The next steps involve rigorous testing to pinpoint the areas where the algorithm is exhibiting incorrect behavior and to refine its performance.

## Code Planning
In our particle filter implementation, we've adopted a structured approach centered around the primary node pf.py. This central node is responsible for managing key components of the system, including a Map of the MAC, robot movement, and LIDAR data on the map. These components collectively enable the particle filter to perform its localization task effectively.

In our model, the Map of the Mac is responsible for representing and maintaining the map of the environment. It serves as a reference for the robot to understand its surroundings and make informed decisions. Robot movement encompasses the tracking of the robot's movement using odometry readings. It helps predict the potential positions of the robot based on its past actions and movements. The Lidar data on the map deals with integrating lidar sensor data, which is crucial for estimating the robot's position and orientation within the map. The ParticleFilter node efficiently manages the subscription and publication to various ROS (Robot Operating System) topics, facilitating the exchange of information between different components. It also handles the distribution of particles, maintaining a list of "ParticleDistribution" objects, which collectively represent potential robot poses. This architectural design allows for a streamlined and modular approach to particle filtering, enhancing the maintainability and expandability of the system while ensuring that the particle filter can accurately estimate the robot's position within the given environment.

![image](https://github.com/MihirV17/robot_localization/assets/123433158/9720f5a2-0bbe-40bb-8ec1-2fbfae77d412)

## Code Implementation
