cmake_minimum_required(VERSION 3.3)
project(softkinetic)

set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -std=c++11")

set(SOURCE_FILES
    softkinetic/CMakeLists.txt
    softkinetic/package.xml
    softkinetic_camera/cfg/Softkinetic.cfg
    softkinetic_camera/cmake/FindDepthSenseSDK.cmake
    softkinetic_camera/config/softkinetic_camera_ds311.yaml
    softkinetic_camera/launch/softkinetic.rviz
    softkinetic_camera/launch/softkinetic_camera_demo.launch
    softkinetic_camera/launch/softkinetic_camera_ds311.launch
    softkinetic_camera/launch/softkinetic_camera_ds311_demo.launch
    softkinetic_camera/launch/softkinetic_camera_ds325.launch
    softkinetic_camera/launch/softkinetic_cameras.launch
    softkinetic_camera/meshes/asus_xtion_pro_live.dae
    softkinetic_camera/meshes/asus_xtion_pro_live.png
    softkinetic_camera/resources/senz3d.yaml
    softkinetic_camera/src/softkinetic_start.cpp
    softkinetic_camera/urdf/senz3d.urdf.xacro
    softkinetic_camera/CMakeLists.txt
    softkinetic_camera/package.xml
    softkinetic_camera/README.md)

add_executable(softkinetic ${SOURCE_FILES})