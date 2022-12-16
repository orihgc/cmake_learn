cmake_minimum_required(VERSION 3.0)
#project:定义工程名称，隐式定义PROJECT_BINARY_DIR和PROJECT_SOURCE_DIR
project(cmake_learn)
#SET显示地定义变量
set(CMAKE_CXX_STANDARD 14)

#message 输出用户自定义信息
#SEND_ERROR，产生错误，生成过程被跳过。
#STATUS，输出前缀为—的信息。
#FATAL_ERROR，立即终止所有 cmake 过程.
message(STATUS "This is BINARY dir" ${PROJECT_BINARY_DIR})
message(STATUS "This is SOURCE dir" ${PROJECT_SOURCE_DIR})

#生成一个名为cmake_learn的可执行文件，相关源文件是main.cc
add_executable(cmake_learn main.cpp)
