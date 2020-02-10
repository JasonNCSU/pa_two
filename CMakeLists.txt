cmake_minimum_required(VERSION 2.8.8)
project(two)

add_library(src "src/main.cpp" "src/vectorAdd.cu")

add_executable(main "src/main.cpp")
target_link_libraries(main src)