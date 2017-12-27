# DR2
ISR-Lab project 2017

### What we are going to do:
The robot we are going to work on is the Kobuki.
We are going to use its depth camera with ROS environment, in order to use it in AI (so it will be compatible with SWI-Prolog, SICStus Prolog and DALI).

### Needed hardware:
1. Kobuki robot
2. JetsonTK1 board
3. Orbbec Astra 3D Camera

### Software constraints:
We will use Python, Prolog and ROS.
We are going to follow the Sense-Think-Act paradigm.
We will use Docker to avoid compatibility conflicts.

### TO DO:
1. Reconfigure JetsonTK1 board (Done)
2. Configure Orbbec Astra 3D Camera (Done)
3. Create a communication channel between the camera and ROS environment
4. Create a Docker container with all the needed environment in it to avoid compatibility conflicts (Done)
5. Integrate Prolog in ROS environment
6. Create a simulation and run it on the robot
5. (Optional) Facial recognition ability

### Use case 1:
Kobuki goes around into the room, avoiding obstacles and "looking" around thanks to the camera.
Kobuki is able to forward camera data to its Prolog brain.

### (Optional) Use case 2:
Kobuki goes around into the room, avoiding obstacles and "looking" around thanks to the camera.
Kobuki is able to forward camera data to its Prolog brain.
Kobuki is able to detect people face and to recognize them (by making queries to its Prolog brain).

### Links:
-  http://www.nvidia.it/object/jetson-tk1-embedded-dev-kit-it.html
-  https://developer.nvidia.com/embedded/jetpack
-  https://demotomohiro.github.io/hardware/jetson_tk1/setup/recovery_mode.html
#### Software Links:
-  https://github.com/agnsal/docker-IndigoROSdisPyPl: we have to use ROS Indigo (inside a Docker container, because Indigo is not compatible with Ubuntu 16.04, that we have on our PCs); we have Ubuntu 14.04 on JetsonTK1 board, because it is needed by CUDA.
-  http://wiki.ros.org/kinetic/Installation/Ubuntu


## Instructions:
1. Follow the instructions at https://github.com/agnsal/docker-IndigoROSdisPyPl.
2. **Install turtlebot ROS packages:** \
  sudo apt-get install ros-indigo-turtlebot ros-indigo-turtlebot-apps ros-indigo-turtlebot-interactions ros-indigo-turtlebot-   simulator ros-indigo-kobuki-ftdi ros-indigo-rocon-remocon ros-indigo-rocon-qt-library ros-indigo-ar-track-alvar-msgs
