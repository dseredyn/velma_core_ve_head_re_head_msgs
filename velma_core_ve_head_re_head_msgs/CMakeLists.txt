cmake_minimum_required(VERSION 2.8.6)

project(velma_core_ve_head_re_head_msgs)

find_package(catkin REQUIRED
  COMPONENTS std_msgs geometry_msgs message_generation actionlib_msgs)

add_message_files(FILES
  Command.msg
  Status.msg
  )
  

generate_messages(
  DEPENDENCIES
  std_msgs
  geometry_msgs
  )


catkin_package(
  CATKIN_DEPENDS std_msgs geometry_msgs message_runtime)
