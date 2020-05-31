cmake_minimum_required(VERSION 3.10)

# set the project name
project(OpenSprinkler C++11)

add_compile_definitions(OpenSprinkler OSPI=1)
add_executable(OpenSprinkler main.cpp OpenSprinkler.cpp program.cpp server.cpp utils.cpp weather.cpp gpio.cpp etherport.cpp)
target_link_libraries(OpenSprinkler pthread)

