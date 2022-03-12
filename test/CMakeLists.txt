add_executable(${CMAKE_PROJECT_NAME}_test main.cpp)

add_test(NAME ${CMAKE_PROJECT_NAME}_test COMMAND ${CMAKE_PROJECT_NAME}_test)

target_link_libraries(${CMAKE_PROJECT_NAME}_test PUBLIC ${CMAKE_PROJECT_NAME}_lib gtest)
