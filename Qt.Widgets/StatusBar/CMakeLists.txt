cmake_minimum_required(VERSION 3.1)

# Project
project(StatusBar)
find_package(Qt5Widgets CONFIG REQUIRED)

# Options
set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

# Application
add_executable(StatusBar WIN32 MACOSX_BUNDLE src/StatusBar.cpp)
target_link_libraries(StatusBar Qt5::Widgets)
