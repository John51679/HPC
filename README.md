# HPC
This project was created as part of "Software and programming of high performance systems" subject in Computer Engineering & Informatics Department (CEID) of University of Patras. It uses C and Cuda to perform the calculation of 
$$A^T \cdot A$$
where A is a given matrix.

It attempts the calculation in three ways
- `HPC_task_1.cu`: Performs the multiplication using the cuBLAS library that cuda provides
- `HPC_task_2.cu`: Performs the multiplication using a user defined function
- `HPC_task_3.cu`: Performs the multiplication using an optimized version of the user defined function

For the functions we have created:
1. init():
  Initializes the dimensions of the table, taking values from the keyboard.
2. GPU_fill_rand():
  Fills the table with values using either curand()(GPU)
3. table_generator():
  Fills the table with values using either rand()(CPU)
4. print_matrix():
  Prints on the screen the elements of the input matrix.
5. gpu_blas_mmul()
  Performs the necessary calculations using the cuBLAS library
6. __global__ void kernel():
  Performs the necessary calculations using the user-defined function with or without optimizations.
7. main():
  Calls the necessary command-functions to implement the the corresponding algorithm.
