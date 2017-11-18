cmake_minimum_required(VERSION 2.8.3)
project(hark_msgs)

find_package(catkin REQUIRED COMPONENTS
  message_generation
  std_msgs
)

add_message_files(
  FILES
  HarkFeature.msg
  HarkInt.msg
  HarkSource.msg
  HarkSrcFeature.msg
  HarkSrcWave.msg
  HarkFeatureVal.msg
  HarkJulius.msg
  HarkSourceVal.msg
  HarkSrcFeatureVal.msg
  HarkSrcWaveVal.msg
  HarkFFT.msg
  HarkJuliusSrc.msg
  HarkSrcFeatureMFM.msg
  HarkSrcFFT.msg
  HarkWave.msg
  HarkFFTVal.msg
  HarkJuliusSrcVal.msg
  HarkSrcFeatureMFMVal.msg
  HarkSrcFFTVal.msg
  HarkWaveVal.msg
)

add_service_files(
  FILES
  HarkIntSrv.srv
)

generate_messages(
  DEPENDENCIES
  std_msgs
)

catkin_package(
  CATKIN_DEPENDS message_runtime std_msgs
)
