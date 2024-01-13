cmake_minimum_required(VERSION 3.27.0)

project(HelloOpenCL)

add_executable(${PROJECT_NAME} array_addition.cpp)

target_link_libraries(${PROJECT_NAME} PRIVATE OpenCL::OpenCL)

# set_target_properties(${PROJECT_NAME} PROPERTIES C_STANDARD 11
#                                                  C_STANDARD_REQUIRED ON
#                                                  C_EXTENSIONS OFF)