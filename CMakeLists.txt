cmake_minimum_required(VERSION 3.12)
project(Util)

set(CMAKE_CXX_STANDARD 17)

add_library(Util Tuple.cpp Tuple.h Interval.cpp Interval.h Swap.cpp Swap.h Permutation.cpp Permutation.h Subset.cpp Subset.h SubsetFromList.cpp SubsetFromList.h RandomNormalizedArray.cpp RandomNormalizedArray.h)

add_executable(Test Tuple.cpp Tuple.h Interval.cpp Interval.h Swap.cpp Swap.h Permutation.cpp Permutation.h Subset.cpp Subset.h SubsetFromList.cpp SubsetFromList.h RandomNormalizedArray.cpp RandomNormalizedArray.h Test/catch.hpp Test/PermutationTest.cpp Test/SubsetTest.cpp Test/SubsetFromListTest.cpp Test/RandomNormalizedArrayTest.cpp)