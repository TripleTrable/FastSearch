
add_executable(${CMAKE_PROJECT_NAME}  main.c indexer.c misc.c)
add_library(${CMAKE_PROJECT_NAME}_lib main.c indexer.c misc.c)

target_link_libraries(${CMAKE_PROJECT_NAME} cargs)
