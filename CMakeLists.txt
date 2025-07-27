cmake_minimum_required(VERSION 3.20...3.28.3)

project(P_BOOST_FOR_UG4)

# Compile boost only for 'INTERNAL_BOOST'
if (INTERNAL_BOOST)

    set(FILESYSTEM_SOURCES
            filesystem/src/codecvt_error_category.cpp
            filesystem/src/operations.cpp
            filesystem/src/path.cpp
            filesystem/src/exception.cpp
            filesystem/src/directory.cpp
            filesystem/src/path_traits.cpp
            filesystem/src/portability.cpp
            filesystem/src/unique_path.cpp
            filesystem/src/utf8_codecvt_facet.cpp
            filesystem/src/windows_file_codecvt.cpp
    )

    set(SERIALIZATION_SOURCES
            serialization/src/archive_exception.cpp
            serialization/src/basic_archive.cpp
            serialization/src/basic_iarchive.cpp
            serialization/src/basic_iserializer.cpp
            serialization/src/basic_oarchive.cpp
            serialization/src/basic_oserializer.cpp
#            serialization/src/basic_pointer_iserializer.cpp
#            serialization/src/basic_pointer_oserializer.cpp
            serialization/src/basic_serializer_map.cpp
            serialization/src/basic_text_iprimitive.cpp
            serialization/src/basic_text_oprimitive.cpp
#            serialization/src/basic_xml_archive.cpp
#            serialization/src/binary_iarchive.cpp
#            serialization/src/binary_oarchive.cpp
#            serialization/src/codecvt_null.cpp
#            serialization/src/extended_type_info_no_rtti.cpp
             serialization/src/extended_type_info_typeid.cpp
             serialization/src/extended_type_info.cpp
#            serialization/src/polymorphic_iarchive.cpp
#            serialization/src/polymorphic_oarchive.cpp
#            serialization/src/stl_port.cpp
             serialization/src/text_iarchive.cpp
             serialization/src/text_oarchive.cpp
#            serialization/src/utf8_codecvt_facet.cpp
             serialization/src/void_cast.cpp
#            serialization/src/xml_archive_exception.cpp
#            serialization/src/xml_iarchive.cpp
#            serialization/src/xml_oarchive.cpp
#            serialization/src/xml_grammar.cpp
    )

 #add_subdirectory(boost/libs/system)
#            set(SYSTEM_SOURCES
#            system/src/error_code.cpp
#    )

    EXPORTSOURCES(../externals/BoostForUG4/boost/libs/ ${FILESYSTEM_SOURCES})
    EXPORTSOURCES(../externals/BoostForUG4/boost/libs/ ${SERIALIZATION_SOURCES})
#    EXPORTSOURCES(../externals/BoostForUG4/boost/libs/ ${SYSTEM_SOURCES})

else ()

endif ()