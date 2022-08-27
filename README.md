# Ai-robotics-week-6-tasks
Task 5: running and navigation with turtelbot3

![Turtlebot3-waffle-Pi](https://user-images.githubusercontent.com/101488769/185805836-278ff90c-43ae-485b-98c9-51817b9aebf8.png)

### Table of Contents:
1- [Launch Simulation World](#1-Launch-Simulation-World) </br>
2- [Run Navigation Node](#2-Run-Navigation-Node) </br>
3- [Set Navigation Goal](#3-Set-Navigation-Goal) </br>

## 1-Launch-Simulation-World
Navigation is to move the robot from one location to the specified destination in a given environment. For this purpose, a map that contains geometry information of furniture, objects, and walls of the given environment is required. As described in the previous <b> SLAM </b> section, the map was created with the distance information obtained by the sensor and the pose information of the robot itself. </br>

<b> Please use the proper keyword among `burger` , `waffle` , `waffle_pi` for the TURTLEBOT3_MODEL parameter. </b> 
<br/>
<br/>

```$ export TURTLEBOT3_MODEL=waffle```

```$ roslaunch turtlebot3_gazebo turtlebot3_world.launch.```
</br>
</br>

![01](https://user-images.githubusercontent.com/101488769/185805169-475a2471-dc20-4f4f-a0a3-7b8c63eea5aa.png)
</br>
</br>


## 2-Run-Navigation-Node
<B> Open a new terminal from Remote PC with `Ctrl` + `Alt` + `T` and run the Navigation node. <br/>
Please use the proper keyword among `burger` , `waffle` , `waffle_pi` for the TURTLEBOT3_MODEL parameter. </b>
<br/>
<br/>

```$ export TURTLEBOT3_MODEL=waffle```

```$ roslaunch turtlebot3_navigation turtlebot3_navigation.launch map_file:=$HOME/map.yaml```
</br>
</br>

![02](https://user-images.githubusercontent.com/101488769/185805208-48f28fd6-b6d2-4b31-a107-7175e3ce4db1.png)
</br>
</br>


## 3-Set-Navigation-Goal
Click the `2D Nav Goal` button in the RViz menu. Click on the map to set the destination of the robot and drag the green arrow toward the direction where the robot will be facing
</br>
</br>

![task 05~1](https://user-images.githubusercontent.com/101488769/185805701-93c341f7-d1c7-48c6-b3f4-a1d942d1a21a.gif)
</br>
</br>
