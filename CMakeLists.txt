cmake_minimum_required(VERSION 3.10)

project(Marigold)

# -----------------------------------------------------------------------------
# Extra Compile Flags

# Select C++17 as the standard for C++ projects.
set(CMAKE_CXX_STANDARD 17)
# If C++17 is not available, downgrading to an earlier standard is NOT OK.
set(CMAKE_CXX_STANDARD_REQUIRED ON)
# Do not enable compiler specific language extensions.
set(CMAKE_CXX_EXTENSIONS OFF)

# -----------------------------------------------------------------------------
# Copy clang format files

configure_file(${CMAKE_SOURCE_DIR}/.clang-format ${CMAKE_BINARY_DIR}/.clang-format COPYONLY)

# -----------------------------------------------------------------------------
# Add Subdirectories

add_subdirectory(extern)
add_subdirectory(intern)
add_subdirectory(source)
