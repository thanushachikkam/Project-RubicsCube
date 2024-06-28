cmake_minimum_required(VERSION 3.20)
project(rubiks_cube_solver)

set(CMAKE_CXX_STANDARD 14)

include_directories(Model Solver PatternDatabases)

add_executable(rubiks_cube_solver
        Model/RubiksCube.cpp
        Model/RubiksCube.h
        main.cpp Model/RubiksCube3dArray.cpp Model/RubiksCube1dArray.cpp Model/RubiksCubeBitboard.cpp Solver/DFSSolver.h Solver/BFSSolver.h Solver/IDDFSSolver.h Model/PatternDatabase/PatternDatabase.h Solver/IDAstarSolver.h PatternDatabases/NibbleArray.cpp PatternDatabases/NibbleArray.h PatternDatabases/PatternDatabase.cpp PatternDatabases/PatternDatabase.h PatternDatabases/PermutationIndexer.h PatternDatabases/CornerPatternDatabase.cpp PatternDatabases/CornerPatternDatabase.h PatternDatabases/CornerDBMaker.cpp PatternDatabases/CornerDBMaker.h PatternDatabases/math.cpp PatternDatabases/math.h)

# cmake_minimum_required(VERSION 3.20)
# project(rubiks_cube_solver)

# set(CMAKE_CXX_STANDARD 14)

# # Include directories
# include_directories(Model PatternDatabases Solver)

# # Add source files
# set(SOURCES
#     main.cpp
#     Model/RubiksCube.cpp
#     Model/RubiksCube3dArray.cpp
#     Model/RubiksCube1dArray.cpp
#     Model/RubiksCubeBitboard.cpp
#     PatternDatabases/NibbleArray.cpp
#     PatternDatabases/PatternDatabase.cpp
#     PatternDatabases/CornerPatternDatabase.cpp
#     PatternDatabases/CornerDBMaker.cpp
#     PatternDatabases/math.cpp
# )

# # Add header files for better IDE support (optional)
# set(HEADERS
#     Model/RubiksCube.h
#     Model/RubiksCube3dArray.h
#     Model/RubiksCube1dArray.h
#     Model/RubiksCubeBitboard.h
#     Solver/DFSSolver.h
#     Solver/BFSSolver.h
#     Solver/IDDFSSolver.h
#     Solver/IDAstarSolver.h
#     PatternDatabases/NibbleArray.h
#     PatternDatabases/PatternDatabase.h
#     PatternDatabases/CornerPatternDatabase.h
#     PatternDatabases/CornerDBMaker.h
#     PatternDatabases/math.h
#     PatternDatabases/PermutationIndexer.h
# )

# # Add executable
# add_executable(rubiks_cube_solver ${SOURCES} ${HEADERS})
