
set(SRC_DIR src)

set(SRC_FILES
  ${SRC_DIR}/mvt.c
)

add_executable(MVT ${SRC_FILES})
add_dependencies(Polybench MVT)

add_dependencies(supported MVT)

add_test(Polybench_MVT MVT)
