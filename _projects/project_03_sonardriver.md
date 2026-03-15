---
title: "ROS2 Driver for Blueprint Oculus M3000d Imaging Sonar"
excerpt: "<img align='left' src='/images/projects/ProjectSonar.png' width='450' style='margin-right: 15px; margin-bottom: 15px;'/>**PhD Research Project - Ongoing** <br>
Hardware Interface Project - 2025 <br>
C++ - ROS2 - Sensor Driver <br>
Developed a ROS2 C++ driver for the recent blueprint oculus M3000d imaging sonar
(from official M3000d sdk and M1200d ENSTA driver).
Integrated additional acoustic processing on raw sonar data. 
Implemented accurate representation conversion (polar to cartesian)
and point cloud broadcasting.
Tested sonar internal AHRS and pressure sensors. 
Other features are under development-testing based on our needs. "
collection: portfolio
---

**Ongoing** - 2026 | C++ - ROS 2  - Imaging Sonar - Sensor Driver - Underwater Acoustics <br><br>
This project is adapted and extended from the M1200d [ROS2 Driver](https://github.com/godardma/oculus_ros2/tree/main) by ENSTA Bretagne Robotics, and the underlying low level Driver [Sonar Interface](https://github.com/ENSTABretagneRobotics/oculus_driver). The rebase to the M3000d model has been possible thanks to the ViewPointv2 SDK that the Blueprint Subsea Customer Support Team shared with me. 

<div style="display: flex; justify-content: center; align-items: center; gap: 5px; margin-bottom: 5px;">
  <img style="width: 35%; max-width: 500px;" src="/images/projects/03_sonar/sonar01.jpg">
  <img style="width: 22%; max-width: 500px;" src="/images/projects/03_sonar/sonar02.png">
  <img style="width: 35%; max-width: 500px;" src="/images/projects/03_sonar/sonar03.png">
</div>

During the development of the driver, the following tasks have been addressed: 

- Investigated the working principles of acoustic sensing, related software interface, and used data structures.
- Updated the ROS2 driver of the previous sonar model, based on the proprietary C++ SDK.
- Integrated acoustic data pre‑processing and explored possible state estimation approaches

