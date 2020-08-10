add_library(bdshemu SHARED bdshemu.c)
target_include_directories(bdshemu PRIVATE ../inc ../bddisasm/include)
