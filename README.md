## End-to-end autonomy (HRI, Perception, Planning, Navigation, Manipulation, Controls) on a Stretch RE1 robot

This was my Master's capstone project at CMU Robotics. It involved developing and integrating an end-to-end autonomy stack for an indoor assistive robot.

_Project video:_ https://www.youtube.com/watch?v=Km9_RogBT0A <br />
_Project website:_ https://mrsdprojects.ri.cmu.edu/2023teamf <br />
_Project Github:_ https://github.com/Auxilio-Robotics/alfred-deployed

The user provides a voice command to Alfred (Stretch RE1 robot) for fetching an object. Alfred understands this command, plans and navigates to the object's approximate location in the environment, scans for the object, detects the object, identifies grasp points, picks up the object and finally returns back to the user with the desired object. 

- For HRI, we are using Google Cloud Speech-to-Text API and the ChatGPT API. 
- For Navigation, we are using ROS Movebase, STVL for 3D Obstacle Avoidance, GMapping for 2D Lidar SLAM, AMCL for 2D Localization, A* for global planning and DWA for local planning.
- For Perception and Manipulation, we are using Yolo v8, Graspnet and have implemented multiple finite state machines.
- For overall system integration, we have a system-level finite state machine.
- For low-level joint control, we are leveraging the Stretch RE1's open-source APIs.

**My primary role in this project has been:** 
- Use ROS / C++ / Python to set up and optimize the navigation stack (localization, planning & 3D obstacle avoidance)
- Designed & implement a robust software architecture which integrates a cloud-server, HRI interfaces, navigation / manipulation stacks and a high-level task planner.
- Through the course of the project, I have also contributed to various perception, manipulation and system-integration aspects of the project.

<img src = "https://github.com/shivamtrip/assistive-robot/assets/66013750/14234b28-ac6d-40ec-b1de-346036927dd9" width="400"> <br />

Navigation             |  Manipulation
:-------------------------:|:-------------------------:
<img src="https://github.com/shivamtrip/assistive-robot/assets/66013750/1e100290-46ea-495f-a957-8b471560a2af" width="300"> | <img src="https://github.com/shivamtrip/assistive-robot/assets/66013750/70ea1de4-8b33-4bba-8c48-f97217c494ce" width="200">
<img src="https://github.com/shivamtrip/assistive-robot/assets/66013750/a8193a54-35c2-475d-b4ac-610d60c80ebc" width="300">   ![](https://...Ocean.png)





