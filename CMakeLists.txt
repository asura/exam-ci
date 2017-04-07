cmake_minimum_required(VERSION 3.1 FATAL_ERROR)
# CMAKE_CXX_STANDARD : v3.1-

project(exam-ci)

set (CMAKE_CXX_STANDARD 11)

include_directories(
  ${PROJECT_SOURCE_DIR}
  ${PROJECT_SOURCE_DIR}/vendor/Catch/single_include
)

add_executable(
  Tester
  tester.cpp
  shared_ptr_test.cpp
  success_test.cpp
)
