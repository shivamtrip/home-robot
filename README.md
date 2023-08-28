# End-to-end autonomy (HRI, Perception, Planning, Navigation, Manipulation, Controls) on a Stretch RE1 robot

This is an ongoing team project, therefore the code for this project is still private. 

## High-level project overview:
**Developing and integrating the end-to-end autonomy stack for an indoor assistive robot.**

_Link to video:_ https://www.youtube.com/watch?v=Km9_RogBT0A

The user provides a voice command to Alfred (Stretch RE1 robot) for fetching an object. Alfred understands this command, plans and navigates to the object's approximate location in the environment, scans for the object, detects the object, identifies grasp points, picks up the object and finally returns back to the user with the desired object. 

- For HRI, we are using Google Cloud Speech-to-Text API and the ChatGPT API. 
- For Navigation and obstacle avoidance, we are using ROS, Movebase, 2D Lidar slam and other frameworks / algorithms.
- For Perception and manipulation, we are using Yolo v8, Graspnet and have implemented multiple finite state machines.
- For overall system integration, we have a system-level finite state machine.
- For low-level joint control, we are leveraging the Stretch RE1's open-source APIs.

My primary role in this project has been to set up, test and optimize the navigation subsytem. Through the course of the project, I have also contributed to various perception, manipulation and system-integration aspects of the project.

<img src="https://github.com/shivamtrip/assistive-robot/assets/66013750/1e100290-46ea-495f-a957-8b471560a2af" width="400"> <br />

<img src="https://github.com/shivamtrip/assistive-robot/assets/66013750/70ea1de4-8b33-4bba-8c48-f97217c494ce" width="200">
