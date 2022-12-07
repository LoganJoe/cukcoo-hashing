cmake_minimum_required(VERSION 3.23)
project(cuckoo_hashing CUDA)

set(CMAKE_CUDA_STANDARD 17)

add_executable(cuckoo_hashing main.cu include/hash_table.h)

set_target_properties(cuckoo_hashing PROPERTIES
        CUDA_SEPARABLE_COMPILATION ON)
