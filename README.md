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
>* protoc 3.0.0
>* python 3.6

## Fetch Flightmare and Dependency
>* mkdir ~/FlightmareRepos && cd ~/FlightmareRepos
>* repo init --no-repo-verify -u https://github.com/kongdaqing/SimFlightmare.git -m default.xml -b master
>* repo sync
 
## Build Flightmare
>* cd src
>* catkin_init_workspace
>* catkin_make

## Download Unity Binary
>* Click [the link](https://flightmare.readthedocs.io/en/latest/getting_started/quick_start.html) and find title **Download Flightmare Unity Binary**,then click **Download** buttom to download the Flightmare Unity Binary RPG_Flightmare.tar.xz for rendering from the Releases and extract it into the ~/FlightmareRepos/src/flightmare/flightrender.

## Run Flightmare
>* source devel/setup.zsh
>* roslaunch flightros rotors_gazebo.launch

## First Fly
 You will see coarse quadrotor model in the gazebo and realistic quadrotor and enviroment model in the unity,**RPG QUADROTOR GUI** display states of quadrotor.
>* connect joystick
>* click **connect** bottom on the **RPG QUADROTOR GUI**
>* click "Arm Bridge" and control quadrotor with joystick
![](https://github.com/kongdaqing/SimFlightmare/raw/master/pictures/flightmare_run.png)


