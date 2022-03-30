set(CMAKE_VERBOSE_MAKEFILE ON)
cmake_minimum_required (VERSION 3.19.0)
project (CUDA_PLAYGRROUND CUDA)
set(CMAKE_CUDA_ARCHITECTURES 75)
file(GLOB_RECURSE cudapg_SRC
    "src/*.cu"
)
add_executable(cudapg ${cudapg_SRC})