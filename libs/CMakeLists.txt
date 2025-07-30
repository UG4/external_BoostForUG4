include("../../../ugcore/cmake/ug_cmake_versions.cmake")

project(P_BOOST_FOR_UG4)

# Compile boost only for 'INTERNAL_BOOST'
if(INTERNAL_BOOST)
	add_subdirectory(filesystem)
	add_subdirectory(serialization)
	add_subdirectory(system)
elseif(INTERNAL_BOOST)

endif(INTERNAL_BOOST)
