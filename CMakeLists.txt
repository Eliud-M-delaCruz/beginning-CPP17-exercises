cmake_minimum_required(VERSION 3.10.0)
project(beginning-cpp17-exercises VERSION 0.1.0 LANGUAGES C CXX)

add_subdirectory(Ch02)

set(CPACK_PROJECT_NAME ${PROJECT_NAME})
set(CPACK_PROJECT_VERSION ${PROJECT_VERSION})
include(CPack)