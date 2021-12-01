# Happy Mini TurtleBot3 Simulaitons
## 概　要
次のturtlebot3_simulationsパッケージにhappy miniのモデル(URDF, Mesh)を追加した。現時点では、ロボット台車のパラメータはwaffle_piと同じ。  
- http://wiki.ros.org/turtlebot3_simulations (metapackage)

## 使用法
1. Empty World
- $ export TURTLEBOT3_MODEL=happy_mini
- $ ros2 launch turtlebot3_gazebo empty_world.launch.py

2. TurtleBot3 World
- $ export TURTLEBOT3_MODEL=happy_mini
- $ ros2 launch turtlebot3_gazebo turtlebot3_world.launch.py

3. TurtleBot3 House
- $ export TURTLEBOT3_MODEL=happy_mini
- $ ros2 launch turtlebot3_gazebo turtlebot3_house.launch.py


