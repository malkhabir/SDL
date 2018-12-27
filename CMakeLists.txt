cmake_minimum_required(VERSION 3.12)
project(sdlexperience C)         // <--------------- change sdlexperience with the name of the project or .c file

set(CMAKE_C_STANDARD 99)




find_package(SDL2 REQUIRED)                                        // <----- added 

include_directories(${PROJECT_NAME} ${SDL2_INCLUDE_DIRS})             // <----- added 

add_executable(sdlexperience main.c)                                // <--------------- change sdlexperience with the name of the project or .c file


target_link_libraries(${PROJECT_NAME} ${SDL2_LIBRARIES})               // <----- added order counts
