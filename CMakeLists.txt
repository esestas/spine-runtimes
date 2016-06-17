cmake_minimum_required(VERSION 2.8.9)
project(spine)

set(CMAKE_INSTALL_PREFIX "./")

add_subdirectory(spine-c)
add_subdirectory(spine-sfml)
add_subdirectory(spine-cocos2d-iphone)