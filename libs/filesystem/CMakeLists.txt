cmake_minimum_required(VERSION 2.8.12)

project(P_BOOST_FOR_UG4__FILESYSTEM)

set(SOURCES 
	src/codecvt_error_category.cpp
	src/operations.cpp
	src/path.cpp
	src/path_traits.cpp
	src/portability.cpp
	src/unique_path.cpp
	src/utf8_codecvt_facet.cpp
	src/windows_file_codecvt.cpp
)

EXPORTSOURCES(../externals/BoostForUG4/libs/filesystem ${SOURCES})
