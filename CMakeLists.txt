cmake_minimum_required(VERSION 3.20.0)
project(Hackerrank VERSION 0.1.0 LANGUAGES C CXX)

set(CMAKE_CXX_STANDARD 20)
set(CMAKE_CXX_STANDARD_REQUIRED True)

include(CTest)
enable_testing()

add_executable(Hackerrank Source/main.cpp Source/ProblemsManager/Problem.cpp Source/ProblemsManager/ProblemsManager.cpp)

set(CPACK_PROJECT_NAME ${PROJECT_NAME})
set(CPACK_PROJECT_VERSION ${PROJECT_VERSION})
include(CPack)
