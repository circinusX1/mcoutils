
cmake_minimum_required (VERSION 2.6)
PROJECT(MCOUTIL)


#set(CMAKE_C_COMPILER "gcc")
#set(CMAKE_CXX_COMPILER "g++")

set(CMAKE_CXX_FLAGS "-std=c++0x -Wall -fexceptions -fpermissive -D__USE_MISC")



include_directories ("../mcoutils" "./" "../mcosocks")
ADD_LIBRARY(mcoutil STATIC config.cpp minidb.cpp sslcrypt.cpp)
SET(LIBRARY_OUTPUT_PATH ../lib)


