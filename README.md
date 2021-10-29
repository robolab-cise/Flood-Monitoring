# Flood-Monitoring
- This is a repository for a Robot Operating System (ROS) project.
- The project is for a Voronoi-based flood area detection using multi-agent systems.

## Abstract
An algorithm was made to support detection of connected and disconnected segment of water in a flood area. The algorithm aims to distribute  drones around water of a flood area in a stochastic environment. The algorithm is implemented using Voronoi function and image segmentation. The goal is to provide information regarding the position of water in a flood area with the help of the drones. The Voronoi-based approach use multi-modal Gaussian distribution to generate density around centroids, with centroids closer to water having a higher density. As a result, these centroids will attract other centroids with lower density. Since each centroid is associated with a drone, whenever a centroids' location are updated it will drag their respective drone along with them. Image segmentation assists the algorithm with detecting water in a flood area by differentiating between the color of the ground and the color of the water. We will do a simulation with three disjointed water area and investigate the performance of the algorithm. 

### Note
- READ.md files are Github readme files that are required by the platform.
