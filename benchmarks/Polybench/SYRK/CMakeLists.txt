
set(SRC_DIR src)

set(SRC_FILES
  ${SRC_DIR}/syrk.c
)

add_executable(SYRK ${SRC_FILES})
add_dependencies(Polybench SYRK)

add_dependencies(experiments SYRK)
add_dependencies(supported SYRK)

add_test(Polybench_SYRK SYRK)
