# CMakeLists.txt file generated with DCG.

# To stop file regeneration, remove the following line.
#!DCG_REGENERATE_THIS_FILE

add_executable(DcTestUtilityTest)

set_property(TARGET DcTestUtilityTest PROPERTY FOLDER tests)

target_compile_features(DcTestUtilityTest INTERFACE cxx_std_20)

target_link_libraries(DcTestUtilityTest
PRIVATE
  DcTestUtility
  gmock
  gtest_main
)

set(tst
  "${CMAKE_CURRENT_SOURCE_DIR}/Helpers/TestHelpersTest.cpp"
)

target_sources(DcTestUtilityTest
PRIVATE
  ${tst}
)

source_group(TREE "${CMAKE_CURRENT_SOURCE_DIR}" PREFIX "test" FILES ${tst})

DCG_add_interface_source_group(DcTestUtility)
