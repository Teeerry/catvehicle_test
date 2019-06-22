#Project
人工智能与机器人 2018 秋概率机器人三级项目-选做题 构建无人驾驶仿真系统

# Authors and contributors
* name: Terry 
* email: terryluohello@qq.com

# About
The catvehicle_test ROS package houses files for testing the catvehicle

# Dependencies
* ROS
* obstaclestopper
* catvehicle

# Simple tutorial and examples

1. 方式一(通过按键控制车辆运动)
```
    terminal 1: `roslaunch catvehicle_test atvehicle_visual.launch`

    terminal 2:  `roslaunch turtlebot_teleop keyboard_teleop.launch`
    
    terminal 3:  `rosrun topic_tools relay /cmd_vel_mux/input/teleop /catvehicle/cmd_vel`
```

2. 方式二（通过编写节点控制运动）
```
    terminal 1:  `roslaunch catvehicle_test forward_test.launch`
```