cmake_minimum_required(VERSION 3.18)
project(myapp)

list(APPEND CMAKE_MODULE_PATH "/usr/local/lib/cmake/OpenVDB")
find_package(OpenVDB REQUIRED)

add_executable(myapp src/main.cpp)
target_link_libraries(myapp OpenVDB::openvdb)
