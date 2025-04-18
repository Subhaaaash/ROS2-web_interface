# ROS2-web_interface

#STEP1: INSTALL WEB INTERFACE

``` bash

$ sudo apt install ros-humble-rosbridge-server
```

#STEP2: ADD .html CODE 

``` bash
$ git clone https://github.com/Subhaaaash/ROS2-web_interface.git
```

#STEP3: TERIMINAL 1 --> start server 

``` bash
$ cd ROS2-web_interface
$ python3 -m http.server 8000
```
open the the address given in the concsole and select two_way_com.html


#STEP4: TERMINAL 2 --> start ROS2 web socket 

``` bash
$ ros2 launch rosbridge_server rosbridge_websocket_launch.xml
```
#STEP5: TERMINAL 3 --> start your turtle sim node 

``` bash 
$ ros2 run turtlesim turtlesim_node

```
