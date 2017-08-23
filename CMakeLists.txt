cmake_minimum_required (VERSION 2.8)
project(quickhull)

find_package(catkin_simple REQUIRED)
catkin_simple(ALL_DEPS_REQUIRED)

add_definitions(--std=c++11)

cs_add_library(${PROJECT_NAME} include/QuickHull.cpp)

cs_install()
cs_export()
