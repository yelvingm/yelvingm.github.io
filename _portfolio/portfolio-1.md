---
title: "Autonomous Machine for Inspecting Gas Operations (AMIGO)"
excerpt: "Co-Lead - Company Sponsored Project to <br/><img src='/src/yelvingm.github.io/images/amigo.jpg'>"
collection: portfolio
---

This is a project by the Research and Development Team of Louisiana Steam (hyperlink to Louisiana Steam) with the goal of creating an end-to-end solution for automating inspection tasks of hazardous environments such as oil and gas refineries, chemical plants, and paper mills. 

The project seeks to concentrate innovation in critical areas, including domains such as all terrain navigation, behavior trees, and multimodal sensor fusion.

Sensor Fusion:

![Testing Ublox GPS Module]({{ '/files/GPS_TEST.mp4' | relative_url }})

The sensor array consists of a GPS, a Respeaker Mic Array, LiDAR, and Gas Sensors. Localization is achieved through Kalman Filtering of 3 IMU's and 2 sources of odometry.

Navigation:

![Testing AMIGO's Indoor Obstacle Avoidance]({{ '/files/AMIGO_NAV.mp4' | relative_url }})

Navigation is achieved through a waypoint-based follower provided by Nav2, and open source software stack (Link to Nav2).

User Interface:

![Operator GUI]({{ '/images/monitor.png' | relative_url }})

This project also provides a GUI to operators for analyzing mission execution, sensor inputs, and decision making. The GUI was made with PyQt and ROS2. 

Future Work:

With localization and navigation achieved, we seek to enhance AMIGO's level of autonomy through...

1. Implementing a Behavior Tree to optimize mission scheduling 
2. Training machine learning algorithms to detect acoustic signatures of target sounds from anomolies (Pipe Burst, Gas Leak)
