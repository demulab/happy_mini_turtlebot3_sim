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
$ sudo apt install ros-foxy-gazebo-*
$ sudo apt install ros-foxy-gazebo-ros-pkgs
```
- Turtlebot3関連パッケージのインストール
```
$ sudo apt install ros-foxy-dynamixel-sdk
$ sudo apt install ros-foxy-turtlebot3
$ sudo apt install ros-foxy-turtlebot3-msgs
$ sudo apt install ros-foxy-turtlebot3-gazebo
```
- Happy Mini関連パッケージのインストール
```
$ cd ~/airobot_ws/src
$ git clone https://github.com/AI-Robot-Book/happy_mini_turtlebot3_sim
$ cd ~/colcon_ws
$ colcon build 
```


## 実行
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
4. ロボットモデルの変更
- Waffle Piを使う場合
```
$ export TURTLEBOT3_MODEL=waffle_pi
```

## 著者
出村 公成

## 履歴
- 2022-10-05: Happy miniの3DモデルがLiDARのレーザ光と干渉するので以下のファイルを変更．
  - https://github.com/AI-Robot-Book/happy_mini_turtlebot3_sim/blob/main/turtlebot3_gazebo/models/turtlebot3_happy_mini/model.sdf
- 2022-08-29: 初期版

## ライセンス
Copyright (c) 2022, Kosei Demura All rights reserved. This project is licensed under the Apache License 2.0 license found in the LICENSE file in the root directory of this project.


## 参考文献
- 今のところありません．
