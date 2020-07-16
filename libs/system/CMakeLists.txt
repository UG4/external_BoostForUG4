cmake_minimum_required(VERSION 2.6)

project(P_BOOST_FOR_UG4__SYSTEM)

set(SOURCES 
	src/error_code.cpp
)

EXPORTSOURCES(../externals/BoostForUG4/libs/system ${SOURCES})
