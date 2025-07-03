
# 使用第一代livox雷达（avia）
cd ~/ws_livox/
source devel/setup.bash
cd ~/FAST_LIO/
catkin_make -j20
source devel/setup.bash
roslaunch fast_lio mapping_avia.launch

# 使用第二代lidar（mid360）
cd ~/ws_livox_mid360/
source devel/setup.bash
cd ~/FAST_LIO/
catkin_make -j20
source devel/setup.bash
roslaunch fast_lio mapping_mid360.launch



# 注意，这里的mid360和aiva的驱动路径请根据实际情况修改
# 注意，如果想使用avia请把工程中的“livox_ros_driver2”替换成“livox_ros_driver”
# 注意，如果想使用mid360请把工程中的“livox_ros_driver”替换成“livox_ros_driver2”
