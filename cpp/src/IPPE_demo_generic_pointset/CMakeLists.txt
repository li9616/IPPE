project( IPPE_demo_generic_pointset)
find_package( OpenCV REQUIRED )
include_directories(
    ${OpenCV_INCLUDE_DIRS}
    ${CMAKE_SOURCE_DIR}/include
    )
add_executable( IPPE_demo_generic_pointset
    IPPE_demo_generic_pointset.cpp
)
target_link_libraries( IPPE_demo_generic_pointset IPPE)
