find_package(RapidJSON)

add_executable(disasmtool disasmtool.cpp dumpers.cpp rapidjson.cpp)
target_compile_definitions(disasmtool PRIVATE HAS_RAPIDJSON)
target_include_directories(disasmtool PRIVATE ../inc)
target_compile_features(disasmtool PRIVATE cxx_std_17)
target_link_libraries(disasmtool PRIVATE bddisasm)
