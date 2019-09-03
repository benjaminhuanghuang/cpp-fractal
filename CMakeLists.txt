cmake_minimum_required(VERSION 3.7)

set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -std=c++11 -stdlib=libc++")

project(cpp-fractal)

include_directories(src)
                    
file(GLOB project_SRCS src/*.cpp) #src/*.h

add_executable(main.exe ${project_SRCS})


target_link_libraries(main.exe)