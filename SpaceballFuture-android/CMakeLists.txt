cmake_minimum_required(VERSION 3.0)
include(../../core/CMake/LFLOS.cmake)
include(../../core/CMake/AndroidStudio.cmake)

set(LFL_FLATBUFFERS 1)
set(LFL_FREETYPE 1)
set(LFL_PNG 1)
set(LFL_FABRIC 1)
set(LFL_BOX2D 1)
set(LFL_ICONV 1)
set(LFL_SOURCE_DIR ${CMAKE_CURRENT_SOURCE_DIR}/../..)
set(LFL_BINARY_DIR ${CMAKE_CURRENT_BINARY_DIR})
set(LFL_CORE_BINARY_DIR ${CMAKE_CURRENT_BINARY_DIR}/core)
set(FLATBUFFERS_FLATC_EXECUTABLE $ENV{HOME}/bin/flatc)

include(../../core/CMake/LFLCore.cmake)
add_subdirectory(${CMAKE_CURRENT_SOURCE_DIR}/../../SpaceballFuture ${CMAKE_CURRENT_BINARY_DIR}/SpaceballFuture)
