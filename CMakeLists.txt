cmake_minimum_required(VERSION 3.5)
idf_component_register(
  SRCS 
    src/platform.cpp 
    src/SparkFun_VL53L5CX_IO.cpp 
    src/SparkFun_VL53L5CX_Library.cpp 
    src/vl53l5cx_api.cpp 
    src/vl53l5cx_plugin_detection_thresholds.cpp 
    src/vl53l5cx_plugin_motion_indicator.cpp 
    src/vl53l5cx_plugin_xtalk.cpp
  INCLUDE_DIRS 
    "src/."
  REQUIRES 
    "arduino" # Library requires Arduino
)

project(VL53L5CX)