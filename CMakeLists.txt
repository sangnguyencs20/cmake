cmake_minimum_required(VERSION 3.11...3.30)

project(MyProject VERSION 1.0
                  DESCRIPTION "AH SHIET, HERE WE GO AGAIN"
                  LANGUAGES CXX
)
add_subdirectory(printlib)
add_subdirectory(MyLib)

add_executable(myApp main.cpp)
target_link_libraries(myApp PRIVATE MyLib)

message(CMAKE_PROJECT_DESCRIPTION="${CMAKE_PROJECT_DESCRIPTION}")