project(lib_AtmosphericTurbulence_project)

include_directories ("${PROJECT_SOURCE_DIR}/src")
include_directories ("${PROJECT_SOURCE_DIR}/..")

add_library(AtmosphericTurbulence SHARED AtmosphericTurbulence.c 
AtmosphericTurbulence.h
)

install(TARGETS AtmosphericTurbulence DESTINATION lib)
install(FILES AtmosphericTurbulence.h DESTINATION include)
