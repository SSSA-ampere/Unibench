
set(SRC_DIR src)

set(SRC_FILES
  ${SRC_DIR}/3mm.c
)

add_executable(3MM ${SRC_FILES})
add_dependencies(Polybench 3MM)

add_dependencies(experiments 3MM)
add_dependencies(supported 3MM)

add_test(Polybench_3MM 3MM)
