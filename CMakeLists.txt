cmake_minimum_requireD(VERSION 3.10)
project(how-to-optimize-gemm LANGUAGES C)

set(CMAKE_C_STANDARD 11)

set(srcs src/copy_matrix.c
         src/compare_matrices.c
         src/random_matrix.c
         src/dclock.c
         src/REF_MMult.c
         src/print_matrix.c
         src/test_MMult.c
         src/MMult0.c)

add_executable(${PROJECT_NAME} ${srcs})