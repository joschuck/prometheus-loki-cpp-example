cmake_minimum_required(VERSION 3.24)
project(prometheus_cpp_example)

set(CMAKE_CXX_STANDARD 17)

find_package(prometheus-cpp CONFIG REQUIRED)

add_executable(prometheus_cpp_example main.cpp)
target_link_libraries(prometheus_cpp_example PRIVATE prometheus-cpp::pull)


