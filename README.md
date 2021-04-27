# KUBOT_ROS1_Package 

[![Apache-2.0 License](https://img.shields.io/badge/license-Apache2.0-purple)](http://www.shayangye.com/)
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
[![Platform Badge](https://img.shields.io/badge/platform-ROS_Melodic-blue.svg)](http://www.shayangye.com/)
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
[![version](https://img.shields.io/badge/version-0.0.1-green)](http://www.shayangye.com/)
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
[![robot](https://img.shields.io/badge/robot-KUBOT-orange)](http://www.shayangye.com/)
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;

## Introduction
> ***這是KUBOT機器人共用的ROS workspace，透過腳本選擇機器人、感測器就可以進行仿真、建圖、導航等功能。***


## Installation 

1. [Install ROS](http://wiki.ros.org/ROS/Installation)
2. Create KUBOT  ROS1 workspace 

```sh
git clone https://github.com/KUBOT-Robot/kubot_ros.git
``` 

 - 2.1 Full intsall :
> ***這將完整安裝KUBOT 所有ROBOT的底層驅動、仿真模擬、2D SLAM、3D SLAM、加值裝置等***
> ***此過程需要github金鑰請與專人聯絡***

```sh
./kubot_ros/tools/kubot_install_kubot_all_pkg.sh
./kubot_ros/tools/kubot_install_ros_dep.sh
```


## Initialization environment

```sh
cd ~/kubot_ros/
./kubot_init_env.sh
```

 - 選擇 KUBOT機器人型號
 - 選擇 控制器型號
 - 選擇 激光雷達型號
 - 選擇 深度鏡頭型號
 - 選擇 ROS Master or Slave

```sh
source ~/.bashrc
```

This script uses bash shell by default. If you use other shells, please modify all  [bash]() words in the script.

```sh
cd ~/ros_ws/
catkin_make
source ~/.bashrc
```
接著就可以享受您的機器人 : 
```sh
example : 
roslaunch kubot_navigation nav.launch
kubot_bringup
```

## Repository Contents

## Version History

Suport ROBOT Model : 
Kubot2 (CAGEBOT) # link
Neuronbot2 # link
Wagv # link
Aider # link
Galiray2 # link

## License






|                |ASCII                          |HTML                         |
|----------------|-------------------------------|-----------------------------|
|Single backticks|`'Isn't this fun?'`            |'Isn't this fun?'            |
|Quotes          |`"Isn't this fun?"`            |"Isn't this fun?"            |
|Dashes          |`-- is en-dash, --- is em-dash`|-- is en-dash, --- is em-dash|




```seq
Andrew->China: Says Hello
Note right of China: China thinks\nabout it
China-->Andrew: How are you?
Andrew->>China: I am good thanks!
```
### End
