# SimFlightmare

**SimFlightmare** is manager of all repos about Flightmare which is simulator for studying uav navigation,control and slam etc through **repo tool**.You can install flightmare through [uzh-rpg/flightmare](https://github.com/uzh-rpg/flightmare) driectly,or you can use this repo for quick start.Attention,Flightmare must be installed with ros through this repo.
## Platform 
>* ubuntu18 
>* ros-melodic 
>   * sudo apt-get install libgoogle-glog-dev protobuf-compiler ros-$ROS_DISTRO-octomap-msgs ros-$ROS_DISTRO-octomap-ros ros-$ROS_DISTRO-joy python-vcstool
>* repo tools
>   * mkdir ~/bin && cd ~/bin
>   * curl https://mirrors.tuna.tsinghua.edu.cn/git/git-repo -o repo
>   * echo "export REPO_URL=https://mirrors.tuna.tsinghua.edu.cn/git/git-repo" >> ~/.zshrc
>   * echo "export PATH=~/bin:$PATH" >> ~/.zshrc
>   * chmod a+x ~/bin/repo
>* protoc version-3.0.0

## Fetch Flightmare and Dependency
>* repo init --no-repo-verify -u https://github.com/kongdaqing/SimFlightmare.git -m default.xml -b master
>* repo sync
 
## Build Flightmare
>* cd src
>* catkin_init_workspace
>* catkin_make

## Run Flightmare
>* roslaunch flightros rotors_gazebo.launch


