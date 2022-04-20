cmake_minimum_required(VERSION 3.10)

target_include_directories(cpr PUBLIC  
    $<INSTALL_INTERFACE:include>    
    $<BUILD_INTERFACE:${CMAKE_CURRENT_SOURCE_DIR}>
    $<BUILD_INTERFACE:${PROJECT_BINARY_DIR}/cpr_generated_includes/>)

