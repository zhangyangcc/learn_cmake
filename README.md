# learn_cmake
学习cmake语法的记录
1. [Why Are Catkin Packages Specified as Components?](http://wiki.ros.org/catkin/CMakeLists.txt#Why_Are_Catkin_Packages_Specified_as_Components.3F)
简单来说，通过这种方式，catkin_INCLUDE_DIRS中包括了catkin包和所有组件包的头文件路径，catkin_LIBRARIES同理。
2. find_package只能找一个包，看语法格式。受到了下面代码块的影响
```
find_package(
   roscpp
  rospy
   std_msgs
)
```