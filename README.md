# End-to-end autonomy (HRI, Perception, Planning, Navigation, Manipulation, Controls) on a Stretch RE1 robot

This is an ongoing team project, therefore the code for this project is still private. 

**High-level project overview:** 
Developing and integrating the end-to-end autonomy stack for a indoor asstive robot.

The user provides a voice command to Alfred (Stretch RE1 robot) for fetching an object. Alfred understands this command, plans and navigates to the object's approximate location in the environment, scans for the object, detects the object, identifies grasp points, picks up the object and finally returns back to the user with the desired object. 

- For HRI, we are using Google Cloud Speech-to-Text API and the ChatGPT API. 
- For Navigation and obstacle avoidance, we are using ROS, Movebase, 2D Lidar slam and other frameworks / algorithms.
- For Perception and manipulation, we are using Yolo v8, Graspnet and have implemented multiple finite state machines.
- For overall system integration, we have a system-level finite state machine. 

**Link to video:** https://www.youtube.com/watch?v=Km9_RogBT0A



