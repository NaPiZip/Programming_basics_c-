set(EXE_NAME "060_Chapter_06")

set(CMAKE_CXX_STANDARD 20)

file(GLOB project_SRC
    "*.h"
    "*.hpp"
    "*.hxx"
    "*.c"
    "*.cpp"
)

add_executable(${EXE_NAME} ${project_SRC})
target_link_libraries(${EXE_NAME} gtest gmock)
