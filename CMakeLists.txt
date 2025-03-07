cmake_minimum_required(VERSION 3.10)
project(AgeGenderPrediction)

# 设置C++标准
set(CMAKE_CXX_STANDARD 11)
set(CMAKE_CXX_STANDARD_REQUIRED True)

# 查找OpenCV库
find_package(OpenCV REQUIRED)

# 添加可执行文件
add_executable(AgeGenderPrediction AgeGender.cpp)

# 链接OpenCV库
target_link_libraries(AgeGenderPrediction ${OpenCV_LIBS})