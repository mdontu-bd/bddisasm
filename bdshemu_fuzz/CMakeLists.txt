add_executable(shfuzz bdshemu_fuzzer.c ../bddisasm/crt.c ../bddisasm/bddisasm.c ../bdshemu/bdshemu.c)
target_include_directories(shfuzz PRIVATE ../inc ../inc/bdshemu ../bddisasm/include)
