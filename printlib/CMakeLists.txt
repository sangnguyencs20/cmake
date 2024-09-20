add_library(printlib STATIC print.cpp)

target_include_directories(printlib PUBLIC ${CMAKE_CURRENT_SOURCE_DIR})
