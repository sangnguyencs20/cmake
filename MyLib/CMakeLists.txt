add_library(MyLib STATIC MyLib.cpp)

target_include_directories(MyLib PUBLIC ${CMAKE_CURRENT_SOURCE_DIR})
target_link_libraries(MyLib PUBLIC printlib)
