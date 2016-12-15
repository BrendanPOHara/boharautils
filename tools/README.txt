There are two main tools that I am looking at for static analysis now.

The first one is clang-check. This one is through clang/llvm, and provides
really nice looking output.

clang-check --analyze source0 <source1 source2...>

The second one is cppcheck. This one provides similar coverage to clang-check,
but the output doesn't look quite as great.

cppcheck source0 <source1 source2...>


Null Pointer Checks:
Both seem to catch these.

Memory Leaks:
cppcheck seems to catch this better than clang-check.
