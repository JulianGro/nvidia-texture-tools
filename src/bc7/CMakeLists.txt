PROJECT(bc7)

SET(BC7_SRCS
	avpcl.cpp
	avpcl.h
	avpcl_mode0.cpp
	avpcl_mode1.cpp
	avpcl_mode2.cpp
	avpcl_mode3.cpp
	avpcl_mode4.cpp
	avpcl_mode5.cpp
	avpcl_mode6.cpp
	avpcl_mode7.cpp
	bits.h
	endpts.h
	shapes_three.h
	shapes_two.h
	tile.h
	avpcl_utils.cpp
	avpcl_utils.h)

ADD_LIBRARY(bc7 OBJECT ${BC7_SRCS})
TARGET_LINK_LIBRARIES(bc7 nvcore nvmath)
TARGET_INCLUDE_DIRECTORIES(bc7 PUBLIC ${CMAKE_CURRENT_SOURCE_DIR})
