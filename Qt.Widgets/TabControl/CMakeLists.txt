cmake_minimum_required(VERSION 3.1)

# Project
project(TabControl)
find_package(Qt5Widgets CONFIG REQUIRED)

# Options
set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

# Application
add_executable(TabControl WIN32 MACOSX_BUNDLE src/TabControl.cpp)
target_link_libraries(TabControl Qt5::Widgets)
