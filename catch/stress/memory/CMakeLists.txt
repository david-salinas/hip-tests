# Common Tests - Test independent of all platforms
set(TEST_SRC
    memcpy.cc
    hipMemcpyMThreadMSize.cc
    hipMallocManagedStress.cc
    hipMemPrftchAsyncStressTst.cc
    hipHostMallocStress.cc
)

hip_add_exe_to_target(NAME memory_stress
                      TEST_SRC ${TEST_SRC}
                      TEST_TARGET_NAME stress_test)
