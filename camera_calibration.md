
# 单目相机标定（ROS camera_calibration）

[目录-入门指北](./README.md)


### 标定步骤

以 usb_cam ROS Package 调用 USB相机为例说明。

[ROS WIki#camera_calibration](http://wiki.ros.org/camera_calibration/)

1. 开启相机

    ```
    roslaunch usb_cam xxx.launch
    ```

2. 开启标定程序 

    ```
    rosrun camera_calibration cameracalibrator.py --size 8x6 --square 0.024 image:=/usb_cam/image_raw camera:=/usb_cam
    ```

    指令中的参数说明
    |参数名称 |说明 |
    |---|---|
    |--size 8x6 | 标定板交叉格点数 |
    |--square 0.024 |标定板单格长度/m |
    |image:=/usb_cam/image_raw |标定相机的图像话题 |
    |camera:=/usb_cam | |


3. 移动相机或标定板，完成标定。
   
   标定板文件 [camera_calibration_check108](http://wiki.ros.org/camera_calibration/Tutorials/StereoCalibration?action=AttachFile&do=view&target=check-108.pdf)

    [奶牛快传/cowtransfer.com](https://cowtransfer.com/s/7acaf36cf24f41)    **传输口令** `lay4wj`

   
4. 保存标定得到的相机参数。

    保存的路径为 `~/.ros/camera_info/XXx_camera.yaml`。

### 标定后，矫正畸变

[ROS WIki#image_proc](http://wiki.ros.org/image_proc/)

1. 开启相机，此时将自动加载标定文件yaml。
   (确保使用和校正时的分辨率参数一致)
   
    ```
    roslaunch usb_cam xxx.launch
    ```

2. 使用 image_proc 矫正畸变
   
    ```
    ROS_NAMESPACE=usb_cam rosrun image_proc image_proc
    ```