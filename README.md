# Happy Mini TurtleBot3 Simulations
## 概　要
次のturtlebot3_simulationsパッケージにhappy miniのモデル(URDF, Mesh)を追加した。現時点では、ロボット台車のパラメータはwaffle_piと同じ。  
- http://wiki.ros.org/turtlebot3_simulations (metapackage)


## 環　境  
- ROS2 Foxy

## インストール  
- GazeboをROSで使うためのパッケージのインストール
```
$ source ~/.bashrc
$ sudo apt install ros-foxy-gazebo-ros-pkgs
```
- Turtlebot3関連パッケージのインストール
```
$ sudo apt install ros-foxy-dynamixel-sdk
$ sudo apt install ros-foxy-turtlebot3-msgs
$ sudo apt install ros-foxy-turtlebot3
```
- Happy Mini関連パッケージのインストール
```
$ cd ~/colcon_ws/src
$ git clone https://github.com/demulab/happy_mini_turtlebot3_sim.git
$ cd ~/colcon_ws
$ colcon build --symlink-install
```

## 使用法
1. Empty World  
![happy mini empty world](https://github.com/demulab/happy_mini_turtlebot3_sim/blob/main/happy_mini_empty_world.png "happy mini empty world")

```
$ export TURTLEBOT3_MODEL=happy_mini
$ ros2 launch turtlebot3_gazebo empty_world.launch.py
```

2. TurtleBot3 World  
![happy mini turtlebot3 world](https://github.com/demulab/happy_mini_turtlebot3_sim/blob/main/happy_mini_turtlebot3_world.png "happy mini turtlebot3 world")
```
$ export TURTLEBOT3_MODEL=happy_mini
$ ros2 launch turtlebot3_gazebo turtlebot3_world.launch.py
```

3. TurtleBot3 House
![happy mini turtlebot3 house](https://github.com/demulab/happy_mini_turtlebot3_sim/blob/main/happy_mini_house.png "happy mini turtlebot3 house")
```
$ export TURTLEBOT3_MODEL=happy_mini
$ ros2 launch turtlebot3_gazebo turtlebot3_house.launch.py
```
