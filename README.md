# setup_guide

入门指北

### 总览

[集群系统框架](./Cluster_architecture.md)

### 硬件设备 （使用和说明书）

1. 无人机

[成品平台(四旋翼&小车)](./Vehicles_complete.md)

[自组PX4无人机设备清单](./Vehicles_px4.md)


2. 机载计算机

[机载计算机](./companion_computer.md)

3. 定位系统

[Optitrack室内定位系统](./vrpn_motive.md)

[CUAV RTK](./cuav_rtk.md)

4. 遥控器


5. 充电器


6. 3D 打印机


7. 数据链通信模块

- 超视距串口数据链路模块

  [P900模块配置-Mesh模式](./P900_radio.md)

- AMOV Homer (~路由器)
    
    TODO


### 基础

- Ubuntu 18.04/20.04 LTS

    ```
    terminal
    git
    ssh
    chmod

    vim*
    ```

- 编程
    
    ```    
    C++ 
    Python3
    ```


- ROS 入门

    [ROS_Wiki/Tutorials](http://wiki.ros.org/ROS/Tutorials)

    [古月居](https://www.guyuehome.com/)

    [创客智造](https://www.ncnynl.com/)

    [MOOC/ROS-Academy-for-Beginners](https://github.com/DroidAITech/ROS-Academy-for-Beginners)


    ```
    topic
    msg
    srv
    roslaunch
    param
    tf
    
    rosbag
    rqt
    ```

- Serial Port 串口设备

    ```
    原理
    波特率
    ```

- MAVLink 协议


- PX4 Autopilot User Guide


### 拓展

- PX4 Development


- Qt5 UI界面设计

    [Ros_Qt5_Gui_App](https://github.com/chengyangkj/Ros_Qt5_Gui_App)


- OpenCV 图像处理


- ROS

    ```
    Gazebo 
    Rviz

    ROS2
    ```


- CUDA


- TCP/ UDP


- shell脚本(.sh/bash)


- CMAKE (CMakeLists)


- 线程/进程


- 结构设计 (CAD/SW/UG/CATIA...)   


- 电路设计 (PCB硬件 & STM32软件)


- 协议 CAN/I2C/SPI


- Docker ??


### PX4 无人机相关

- QGC设置

    [通过QGC校准和配置PX4](./px4_qgc_setup.md)

- cam 相机
  
    [单目相机校准](./camera_calibration.md)


### 辅助软件

-   [远程桌面/nomachine](https://www.nomachine.com/)

-   [Markdowm文本编辑器/Typora-收费了!]

-   [VS Code]
    + Markdown Preview Enhanced 替代 Typora

-   [可视化串口工具/cutecom]

-   [Nvidia Jetson/jtop]


### 文档辅助

[Zhihu/文档自动生成工具](https://zhuanlan.zhihu.com/p/377414780)

-   Markdown

-   mermaid 绘图

    [guide/mermaid-js](https://mermaid-js.github.io/mermaid/)

    [mermaid-live-editor](https://mermaid-js.github.io/mermaid-live-editor/)

-   Doxygen (TBD)

    [Doxygen](https://www.doxygen.nl/)

-   ReadTheDocs (TBD)

    [readthedocs](https://readthedocs.org/)
