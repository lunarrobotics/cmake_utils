cmake_minimum_required(VERSION 3.14)
project(cmake_utils)
set(cmake_utils_FOUND TRUE PARENT_SCOPE)
include(cu_add_library.cmake)
include(generate_gitversion.cmake)
install(FILES
        cmake_utils-config.cmake
        cu_add_library.cmake
        generate_gitversion.cmake
    DESTINATION lib/cmake/${PROJECT_NAME})