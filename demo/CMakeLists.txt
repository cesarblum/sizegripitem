INCLUDE_DIRECTORIES(${CMAKE_CURRENT_BINARY_DIR})

SET(sizegripitemdemo_SOURCES ../SizeGripItem.cpp main.cpp)
SET(sizegripitemdemo_HEADERS ../SizeGripItem.h)

QT4_WRAP_CPP(sizegripitemdemo_HEADERS_MOC ${sizegripitemdemo_HEADERS})

ADD_EXECUTABLE(sizegripitemdemo
  ${sizegripitemdemo_SOURCES}
  ${sizegripitemdemo_HEADERS_MOC})

TARGET_LINK_LIBRARIES(sizegripitemdemo ${QT_LIBRARIES})