# SimFlightmare

**SimFlightmare** is manager of all repos about Flightmare which is simulator for studying uav navigation,control and slam etc through **repo tool**.You can install flightmare through [uzh-rpg/flightmare](https://github.com/uzh-rpg/flightmare) driectly,or you can use this repo for quick start.Attention,Flightmare must be installed with ros through this repo.
## Platform 
>* ubuntu18 
>* ros-melodic 
>   * sudo apt-get install libgoogle-glog-dev protobuf-compiler ros-$ROS_DISTRO-octomap-msgs ros-$ROS_DISTRO-octomap-ros ros-$ROS_DISTRO-joy python-vcstool
>* repo tools
>   * sudo apt-get install repo

Before continuing, make sure that your protobuf compiler version is 3.0.0. To check this out, type in a terminal **protoc --version**.
## Fetch Flightmare and Dependency
>* repo init --no-repo-verify -u git@github.com:kongdaqing/SimFlightmare.git -m default.xml -b master
>* repo sync
 
## Build Flightmare
>* cd src
>* catkin_init_workspace
>* catkin_make

## Run Flightmare
>* roslaunch flightros rotors_gazebo.launch


