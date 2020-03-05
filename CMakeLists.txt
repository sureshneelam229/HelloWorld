cmake_minimum_required(VERSION 2.8.9)
project (hello)

#Contains the headers for the project
include_directories(include)

#Can manually add the sources using the set command as follows:
#set(SOURCES src/hello_world.cpp)

#However, the file(GLOB...) allows for wildcard additions:
file(GLOB SOURCES "src/*.cpp")

add_executable(hello ${SOURCES})

#add_executable(hello hello_world.cpp)
