## This repo is manager of all repos about Flightmare which is simulator for studying uav navigation,control and slam etc.You can install flightmare through [uzh-rpg/flightmare!](https://github.com/uzh-rpg/flightmare) driectly,or you can use this repo for quick start.Attention,flightmare must be installed on ros platform through this repo.
### Platform 
>* ubuntu18 
>* ros-melodic 
>* repo tools
>   * sudo apt-get install repo
##＃ Fetch Flightmare and Dependency
>* repo init --no-repo-verify -u git@github.com:kongdaqing/SimFlightmare.git -m default.xml -b master
>* repo sync
##＃ Build Flightmare
>* cd src
>* catkin_init_workspace
>* catkin_make
##＃ Run Flightmare
>* roslaunch flightros rotors_gazebo.launch


