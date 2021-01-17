cmake_minimum_required(VERSION 3.15)
set (CMAKE_CXX_STANDARD 14)
project(dat)


set(CATCH2DIR /home/rarce/ccom3034)

IF(EXISTS ${CATCH2DIR})   
  include_directories(${CATCH2DIR})
  add_executable(dat main.cpp ${CATCH2DIR}/catch_amalgamated.cpp)
else()
  add_executable(dat main.cpp catch_amalgamated.cpp)
endif()


