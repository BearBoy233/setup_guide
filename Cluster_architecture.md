# 集群无人机框架

[目录-入门指北](./README.md)


### 室内（室内定位系统)

1. 主要设备

```
+ 四旋翼无人机 * N  ( PX4/ Crazyflie 2.X/ Parrot Bebop 2 / DJI Tello 等) 
+ WIFI 路由器 * 1  ( 华硕 GT-5300 )
+ 外部定位系统 * 1  ( OptiTrack Motion Capture/ Nooploop LinkTrack UWB 等）
+ 无人机地面站 * 1  ( Ubuntu + ROS) 
```

2. 额外设备

```
+ 机载计算机         ( Nvidia Jetson/ Intel NUC )
+ 数传/图传模块      ( 串口/ 网口 )
+ 遥控器            ( SBUS )
+ 载荷              ( USB免驱动相机 / Intel Realsense D4XX / 激光雷达 / CSI(CMOS Serial Interface)相机 / 云台 / 机械臂... )           
```

3. 主要软件环境
```
Ubuntu LTS  | 18.04   / 20.04 / 22.04
ROS1        | Melodic / Noetic
ROS2(TODO)  |         / Foxy  / Humble
```

```
- OptiTrack Motion Capture  | vrpn_client_ros
- Nooploop LinkTrack UWB    | nlink_parser
```

```
- PX4           MAVROS
- Crazyflie     crazyswarm
- Bebop         bebop_autonomy + multiple_bebops
```

### 室外 (GPS/RTK)

TODO

同上，外部定位系统 换为 GPS。

RTK 需要 地面定位基站 和 串口数传网络支持。