set(TEST_SOURCES
        # add your *.cpp files here
        Tester.cpp
        ../pljit/lex/test/TestLexer.cpp
        ../pljit/semantic/test/TestSemantic.cpp
        ../pljit/syntax/test/TestSyntax.cpp
        ../pljit/test/TestRegisterFunction.cpp)
add_executable(tester ${TEST_SOURCES})
target_link_libraries(tester PUBLIC
        pljit_core
        GTest::GTest)
