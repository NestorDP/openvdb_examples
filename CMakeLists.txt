cmake_minimum_required(VERSION 3.18)
project(openvdb_examples)

list(APPEND CMAKE_MODULE_PATH "/usr/local/lib/cmake/OpenVDB")
find_package(OpenVDB REQUIRED)

add_executable(hello_world src/hello_world.cpp)
target_link_libraries(hello_world OpenVDB::openvdb)

add_executable(writing_grid src/writing_grid.cpp)
target_link_libraries(writing_grid OpenVDB::openvdb)
