
set(SRC_DIR src)

set(SRC_FILES
  ${SRC_DIR}/mat-mul_gpu.c
)

add_executable(mat-mul ${SRC_FILES})
add_dependencies(mgBench mat-mul)

add_dependencies(experiments mat-mul)
add_dependencies(supported mat-mul)

add_test(mgBench_mat-mul mat-mul)
