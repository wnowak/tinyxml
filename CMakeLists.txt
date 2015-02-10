project(tinyxml)
cmake_minimum_required(VERSION 2.8)

add_library(tinyxml 
	tinystr.cpp
	tinyxml.cpp
	tinyxmlerror.cpp
	tinyxmlparser.cpp
)

install(TARGETS tinyxml
	ARCHIVE DESTINATION lib
	LIBRARY DESTINATION lib
	RUNTIME DESTINATION bin
)

install(FILES tinyxml.h
	DESTINATION include
)
