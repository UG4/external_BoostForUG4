include("../../../../ugcore/cmake/ug_cmake_versions.cmake")

project(P_BOOST_FOR_UG4__SYSTEM)

set(SOURCES 
	src/error_code.cpp
)

EXPORTSOURCES(../externals/BoostForUG4/libs/system ${SOURCES})
