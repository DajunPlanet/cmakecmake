cmake_minimum_required(VERSION 3.25 FATAL_ERROR)

project(cmakemake
    VERSION 0.0.1
    DESCRIPTION "a test demo"
    HOMEPAGE_URL "www.123.com"
    LANGUAGES C CXX

    )


list(APPEND CMAKE_MODULE_PATH "${CMAKE_SOURCE_DIR}/cmake")
include(Buildinfo)


add_subdirectory(src)
add_subdirectory(external)
add_subdirectory(docs)
add_subdirectory(test)
add_subdirectory(packaging)



