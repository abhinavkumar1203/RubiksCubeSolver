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
        PatternDatabase/CornerDBMaker.cpp
        PatternDatabase/CornerDBMaker.h
        PatternDatabase/CornerPatternDatabase.cpp
        PatternDatabase/CornerPatternDatabase.h
        PatternDatabase/NibbleArray.cpp
        PatternDatabase/NibbleArray.h
        PatternDatabase/PatternDatabase.cpp
        PatternDatabase/PatternDatabase.h
        PatternDatabase/PermutationIndexer.h
        PatternDatabase/math.cpp
        PatternDatabase/math.h
        "Pattern Databases/CornerDBMaker.cpp"
        "Pattern Databases/CornerDBMaker.h"
        "Pattern Databases/CornerDBMaker.h"
        "Pattern Databases/CornerPatternDatabase.cpp"
        "Pattern Databases/CornerPatternDatabase.h"
        "Pattern Databases/NibbleArray.cpp"
        "Pattern Databases/NibbleArray.h"
        "Pattern Databases/PatternDatabase.cpp"
        "Pattern Databases/PatternDatabase.h"
        "Pattern Databases/PermutationIndexer.h"
        "Pattern Databases/math.cpp"
        "Pattern Databases/math.h"
        Solver/BFSSolver.h
        Solver/DFSSolver.h
        Solver/IDAstarSolver.h
        Solver/IDDFSSolver.h
        main.cpp
)
