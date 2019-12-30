project(tests)

find_package(Boost COMPONENTS unit_test_framework REQUIRED)

add_executable(test1 test.cpp
        ../src/Processors/ConsoleProcessor.cpp
        ../src/Figure.cpp
        ../src/Figures/Trapeze.cpp
        ../src/Figures/Rhombus.cpp
        ../src/Figures/Pentagon.cpp)
target_link_libraries(test1 ${Boost_LIBRARIES})

add_test(NAME Test1 COMMAND test1)