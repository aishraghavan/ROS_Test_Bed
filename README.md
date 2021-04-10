# ROS_Test_Bed
ROS_Test_Bed


# Start core OS(Run always)

'''
roscore
'''

# Create a project directory and build
'''
 cd ros_test_bed/
~/Desktop/ros_test_bed$ mkdir catkin_ws
~/Desktop/ros_test_bed$ ls
catkin_ws
~/Desktop/ros_test_bed$ cd catkin_ws/
~/Desktop/ros_test_bed/catkin_ws$ ls
~/Desktop/ros_test_bed/catkin_ws$ mkdir src
~/Desktop/ros_test_bed/catkin_ws$ ls
src
'''
### Build system
==================
~/Desktop/ros_test_bed/catkin_ws$ catkin_make

>>>>>>>>>>>>>>>>>>>>>>>>

code in src folder

### Activate the pacakge
==========================

~/Desktop/ros_test_bed/catkin_ws/devel$ source setup.bash 


### NOTE: Avoid repetitive task
==========================
echo "source ~/Desktop/ros_test_bed/catkin_ws/devel/setup.bash" >> ~/.bashrc


# Create package `my_robot_tutorials`
=======================================
catkin_create_pkg  my_robot_tutorials roscpp rospy std_msgs


>>>>>>>>>>>>>>>>>>>>>>>>>
### Build system again 
==================
:~/Desktop/ros_test_bed/catkin_ws$ catkin_make


>>>>>>>>>>>>>
# Create new  file - `my_first_node.py` and run
================================================
python my_first_node.py 

>>>> If error, always have "roscore" running in another terminal

#LIST ALL NODES
================

 rosnode list
/rosout

#########################
