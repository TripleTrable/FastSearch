cmake_minimum_required(VERSION 3.22)

project(fastSearch)


set(CMAKE_CXX_STANDARD 11)

include(FetchContent)
FetchContent_Declare(
  googletest
  URL https://github.com/google/googletest/archive/refs/tags/release-1.11.0.zip
)
# For Windows: Prevent overriding the parent project's compiler/linker settings
set(gtest_force_shared_crt ON CACHE BOOL "" FORCE)
FetchContent_MakeAvailable(googletest)


include_directories(src extern/cargs/include)

add_subdirectory(extern/cargs)
add_subdirectory(src)
add_subdirectory(test)
