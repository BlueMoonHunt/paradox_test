cmake_minimum_required(VERSION 3.10.0)
project(paradox_test VERSION 0.1.0 LANGUAGES C CXX)

add_subdirectory(vendor/paradox)

add_library(${PROJECT_NAME} SHARED src/test.cpp)
target_compile_features(${PROJECT_NAME} PRIVATE cxx_std_14)