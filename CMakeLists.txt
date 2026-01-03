cmake_minimum_required(VERSION 4.0)
project(RubiksCubeSolver)

set(CMAKE_CXX_STANDARD 20)

add_executable(RubiksCubeSolver
        "Model/RubiksCube.cpp"
        "Model/RubiksCube.h"
        "Model/PatternDatabase/PatternDatabase.h"
        Model/RubiksCube1dArray.cpp
        Model/RubiksCube3dArray.cpp
        Model/RubiksCubeBitboard.cpp
        Solver/BFSSolver.h
        Solver/DFSSolver.h
        Solver/IDAstarSolver.h
        Solver/IDDFSSolver.h
        "PatternDatabases/CornerDBMaker.cpp"
        "PatternDatabases/CornerDBMaker.h"
        "PatternDatabases/CornerDBMaker.h"
        "PatternDatabases/CornerPatternDatabase.cpp"
        "PatternDatabases/CornerPatternDatabase.h"
        "PatternDatabases/NibbleArray.cpp"
        "PatternDatabases/NibbleArray.h"
        "PatternDatabases/PatternDatabase.cpp"
        "PatternDatabases/PatternDatabase.h"
        "PatternDatabases/PermutationIndexer.h"
        "PatternDatabases/math.cpp"
        "PatternDatabases/math.h"
        Solver/BFSSolver.h
        Solver/DFSSolver.h
        Solver/IDAstarSolver.h
        Solver/IDDFSSolver.h
        main.cpp
)

target_include_directories(RubiksCubeSolver PRIVATE
        ${PROJECT_SOURCE_DIR}
)

target_compile_options(RubiksCubeSolver PRIVATE
        -Wall -Wextra -Wpedantic
)