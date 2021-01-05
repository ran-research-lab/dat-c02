cmake_minimum_required(VERSION 3.15)
project(dat)

set(MyCatch2Dir /home/rarce/ccom3034)
include_directories(${MyCatch2Dir})
add_executable(dat  main.cpp ${MyCatch2Dir}/catch_amalgamated.cpp)

