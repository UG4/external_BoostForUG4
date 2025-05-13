include("../../../../ugcore/cmake/ug_cmake_versions.cmake")


project(P_BOOST_FOR_UG4__SERIALIZATION)

set(SOURCES
  src/archive_exception.cpp
  src/basic_archive.cpp
  src/basic_iarchive.cpp
  src/basic_iserializer.cpp
  src/basic_oarchive.cpp
  src/basic_oserializer.cpp
  src/basic_pointer_iserializer.cpp
  src/basic_pointer_oserializer.cpp
  src/basic_serializer_map.cpp
  src/basic_text_iprimitive.cpp
  src/basic_text_oprimitive.cpp
  src/basic_xml_archive.cpp
  src/binary_iarchive.cpp
  src/binary_oarchive.cpp
  src/codecvt_null.cpp
  src/extended_type_info_no_rtti.cpp
  src/extended_type_info_typeid.cpp
  src/extended_type_info.cpp
  src/polymorphic_iarchive.cpp
  src/polymorphic_oarchive.cpp
  src/stl_port.cpp
  src/text_iarchive.cpp
  src/text_oarchive.cpp
  src/utf8_codecvt_facet.cpp
  src/void_cast.cpp
  src/xml_archive_exception.cpp
  src/xml_iarchive.cpp
  src/xml_oarchive.cpp
  src/xml_grammar.cpp
  # src/basic_xml_grammar.ipp # doesn't show up in "Source Files" in Xcode"'
)

EXPORTSOURCES(../externals/BoostForUG4/libs/serialization ${SOURCES})
