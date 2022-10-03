# Namespace 
ROS allow you to write program in abstract level and control the robot, the communicaton happens through topics.

For a robot it may have information like battery level, position,  odometry, sensor data, etc....

Consider your are naming the topics like    
```
myrobot/battery_status
myrobot/position
myrobot/gps_position
```

If I have to launch two robots, i can launch with another file, but it is redundent and have to hard code names.
```
my_new_robot/battery_status
my_new_robot/position
my_new_robot/gps_position
```

As a solution namespace comes, for first robot set the namespace as `ns="myrobot"` and for second robot set namespace as `ns="my_new_robot"`


## Resources
- http://wiki.ros.org/Names
- https://www.theconstructsim.com/ros-5-mins-046-ros-namespace/
- http://wiki.ros.org/Nodes

## Real Example 
- https://github.com/ROBOTIS-GIT/turtlebot3/blob/master/turtlebot3_navigation/launch/move_base.launch




