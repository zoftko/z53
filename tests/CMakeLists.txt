include(CTest)
include(FetchContent)
FetchContent_Declare(
    googletest
    URL https://github.com/google/googletest/archive/refs/heads/main.zip
)
FetchContent_MakeAvailable(googletest)

add_executable(test_si5351 test_si5351.cc)
target_link_libraries(test_si5351 si5351 gtest_main)
add_test(si5351 test_si5351)
