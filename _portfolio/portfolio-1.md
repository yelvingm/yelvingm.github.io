---
title: "Autonomous Machine for Inspecting Gas Operations (AMIGO)"
excerpt: "Co-Lead: Company Sponsored Project in a Student-Led Laboratory <br/><img src='/images/amigo.jpg' alt='AMIGO'/>"
collection: portfolio
---

This is a project by the Research and Development Team of Louisiana Steam (hyperlink to Louisiana Steam) with the goal of creating an end-to-end solution for automating inspection tasks of hazardous environments such as oil and gas refineries, chemical plants, and paper mills. 

The project seeks to concentrate innovation in critical areas, including domains such as all terrain navigation, behavior trees, and multimodal sensor fusion.

Sensor Fusion:

The sensor array consists of a GPS, a Respeaker Mic Array, LiDAR, and Gas Sensors. Localization is achieved through Kalman Filtering of 3 IMU's and 2 sources of odometry: 1 from Indoor SLAM, and 1 from GPS.

<video controls playsinline preload="metadata" poster="{{ '/images/amigo.jpg' | relative_url }}" width=20vw height=auto class="project-video" loop>
	<source src="{{ '/files/GPS_TEST.mp4' | relative_url }}" type="video/mp4">
	Your browser does not support the video tag. <a href="{{ '/files/GPS_TEST.mp4' | relative_url }}">Download the video</a>.
</video>

![Respeaker Mic Array]({{ '/images/respeaker.jpeg' | relative_url }})

Navigation:

Navigation is achieved through a waypoint-based follower provided by Nav2, and open source software stack (Link to Nav2).

<video controls playsinline preload="metadata" poster="{{ '/images/amigo.jpg' | relative_url }}" width=20vw height=auto class="project-video" loop>
	<source src="{{ '/files/AMIGO_NAV.mp4' | relative_url }}" type="video/mp4">
	Your browser does not support the video tag. <a href="{{ '/files/AMIGO_NAV.mp4' | relative_url }}">Download the video</a>.
</video>

User Interface:

This project also provides a GUI to operators for analyzing mission execution, sensor inputs, and decision making. The GUI was made with PyQt and ROS2. 

![Operator GUI]({{ '/images/monitor.png' | relative_url }})

Future Work:

With localization and navigation achieved, we seek to enhance AMIGO's level of autonomy through...

1. Implementing a Behavior Tree to optimize mission scheduling 
2. Training machine learning algorithms to detect acoustic signatures of target sounds from anomolies (Pipe Burst, Gas Leak)
