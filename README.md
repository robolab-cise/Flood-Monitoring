# Flood-Monitoring
- This is a repository for a Robot Operating System (ROS) project.
- This project is for a Voronoi-based flood area detection using multi-agent systems.

## Abstract
An algorithm was made to support detection of connected and disconnected segment of water in a flood area. The algorithm aims to distribute  drones around water of a flood area in a stochastic environment. The algorithm is implemented using Voronoi function and image segmentation. The goal is to provide information regarding the position of water in a flood area with the help of the drones. The Voronoi-based approach use multi-modal Gaussian distribution to generate density around centroids, with centroids closer to water having a higher density. As a result, these centroids will attract other centroids with lower density. Since each centroid is associated with a drone, whenever a centroids' location are updated it will drag their respective drone along with them. Image segmentation assists the algorithm with detecting water in a flood area by differentiating between the color of the ground and the color of the water. We will do a simulation with three disjointed water area and investigate the performance of the algorithm. 

## How to Download the Folders
The _flood_monitor_ folder we have uploaded to this repository is a folder located inside the _catkin_ws_ folder of the ROS environment. To download the whole folder, find the green **Code** button near the top of the page and click on it. A pop-up menu will appear showing an option to **Download ZIP**. A _flood_monitor.zip_ file will be downloaded to your computer. The zip file will contain all the files and folders listed in this repository under the _flood_monitor_ folder. 

### Note
- README.md files are Github readme files that are required by Github. You can ignore this files when the project folder is copied to _catkin_ws_ folder.
