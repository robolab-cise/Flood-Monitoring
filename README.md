# Flood-Monitoring
- This is a repository for a Robot Operating System (ROS) project.
- This project is for a Voronoi-based flood area detection using multi-agent systems.

## About
An algorithm was made to support detection of connected and disconnected segment of water in a flood area. The algorithm aims to distribute  drones around water of a flood area in a stochastic environment. The algorithm is implemented using Voronoi function and image segmentation. The goal is to provide information regarding the position of water in a flood area with the help of the drones. The Voronoi-based approach use multi-modal Gaussian distribution to generate density around centroids, with centroids closer to water having a higher density. As a result, these centroids will attract other centroids with lower density. Since each centroid is associated with a drone, whenever a centroids' location are updated it will drag their respective drone along with them. Image segmentation assists the algorithm with detecting water in a flood area by differentiating between the color of the ground and the color of the water. We will do a simulation with three disjointed water area and investigate the performance of the algorithm. 

## How to Download the Project Folder
The _flood_monitor_ folder we have uploaded to this repository is a folder located inside the _catkin_ws_ folder of the ROS environment. To download the whole folder, find the green **Code** button near the top of the page and click on it. A pop-up menu will appear showing an option to **Download ZIP**. A _flood_monitor.zip_ file will be downloaded to your computer. The zip file will contain all the files and folders listed in this repository under the _flood_monitor_ folder. 

## How to Install and Run the Simulation
- We assume you have a copy of ROS installed in your machine. Once you have downloaded the project folder, copy it to the folder _catkin_ws/src/_. Open a terminal on your PC and type **_roscore_** and then press Enter, this will start roscore. 
- Next, open another terminal window and type **_roslaunch flood_monitor new_drone_unity.launch_** and then press Enter, this will launch the project's world in Gazebo. You will see Gazebo loading the world into the simulator. Please, add a light source into the world, or else the drones will fail to see the water. Wait for Gazebo to complete loading the world. When the loading is complete, you will see this message displayed in the terminal where you launched Gazebo: **[ WARN] [1636000211.600138404, 28.075000000]: No command received for 28.075s, triggering estop** 
- Finally, open another terminal window, type **_cd catkin_ws/src/flood_monitor/src/_** and then press Enter. Make sure you are in that folder. Then type, **_./test_voronoi.sh_** and then press Enter, to start the simulation. 
- It will take a few seconds to initialize the drones. When the drones are activated you will see small windows pop-up showing the point of view from the drones' camera. When all the drones are in position, the Voronoi function will be executed and another window will pop-up showing the Voronoi and the density diagram. As all of these is taking place, you can see the drones in action in the Gazebo simulator. 
- To stop the simulation, press **_CTRL-C_** on the keyboard for each terminal window except for the Gazebo and roscore terminals. After all the terminals have been terminated, you can then stop Gazebo either from the Gazebo menu or from the Gazebo terminal by pressing **_CTRL-C_**. Then you can shutdown roscore by pressing **_CTRL-C_** on the roscore terminal.

### Note
- README.md files are Github readme files that are required by Github. You can ignore this files when you copy the project folder to the _catkin_ws_ folder.
