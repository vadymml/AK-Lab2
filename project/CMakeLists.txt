add_library(mylib SHARED lib.c)
add_executable(main main.c)
target_link_libraries(main PRIVATE mylib)
target_include_directories(main PRIVATE ${CMAKE_CURRENT_SOURCE_DIR})
