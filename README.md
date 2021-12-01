# Happy Mini TurtleBot3 Simulaitons
## 概　要
次のturtlebot3_simulationsパッケージにhappy miniのモデル(URDF, Mesh)を追加した。現時点では、ロボット台車のパラメータはwaffle_piと同じ。  
- http://wiki.ros.org/turtlebot3_simulations (metapackage)


## 環　境  
- ROS2 Foxy


## 使用法
1. Empty World  
<img src=https://github.com/demulab/happy_mini_turtlebot3_sim/blob/main/happy_mini_empty_world.png" title="happy mini empty world">
- $ export TURTLEBOT3_MODEL=happy_mini
- $ ros2 launch turtlebot3_gazebo empty_world.launch.py

2. TurtleBot3 World  
<img src=https://github.com/demulab/happy_mini_turtlebot3_sim/blob/main/happy_mini_turtlbot3_world.png" title="happy mini turtlebot3 world">     - $ export TURTLEBOT3_MODEL=happy_mini
- $ ros2 launch turtlebot3_gazebo turtlebot3_world.launch.py

3. TurtleBot3 House  
<img src=https://github.com/demulab/happy_mini_turtlebot3_sim/blob/main/happy_mini_house.png" title="happy mini empty world">
- $ export TURTLEBOT3_MODEL=happy_mini
- $ ros2 launch turtlebot3_gazebo turtlebot3_house.launch.py
