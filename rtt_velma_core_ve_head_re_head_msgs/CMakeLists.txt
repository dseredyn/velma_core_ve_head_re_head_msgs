cmake_minimum_required(VERSION 2.8.3)
project(rtt_velma_core_ve_head_re_head_msgs)

find_package(catkin REQUIRED COMPONENTS rtt_roscomm velma_core_ve_head_re_head_msgs eigen_conversions)

find_package(Eigen3 REQUIRED)
include_directories(${Eigen3_INCLUDE_DIR})

ros_generate_rtt_typekit(velma_core_ve_head_re_head_msgs)

orocos_generate_package(
  DEPENDS velma_core_ve_head_re_head_msgs
  DEPENDS_TARGETS rtt_roscomm rtt_std_msgs rtt_geometry_msgs

)
