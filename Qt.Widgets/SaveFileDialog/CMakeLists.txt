cmake_minimum_required(VERSION 3.1)

# Project
project(SaveFileDialog)
find_package(Qt5Widgets CONFIG REQUIRED)

# Options
set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

# Application
add_executable(SaveFileDialog WIN32 MACOSX_BUNDLE src/SaveFileDialog.cpp)
target_link_libraries(SaveFileDialog Qt5::Widgets)
