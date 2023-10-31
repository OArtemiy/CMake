cmake_minimum_required(VERSION 3.26)
project(main VERSION 0.1.0 LANGUAGES C CXX)

set(CMAKE_CXX_STANDARD 17)

include(CTest)
enable_testing()

add_executable(main main.cpp)
set(CMAKE_COLOR_DIAGNOSTICS ON CACHE BOOL "Enable colored diagnostics throughout." FORCE)

set(CPACK_PROJECT_NAME ${PROJECT_NAME})
set(CPACK_PROJECT_VERSION ${PROJECT_VERSION})
include(CPack)
include_directories(~/Code/CppHeaders)
