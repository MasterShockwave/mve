file (GLOB HEADERS "*.h")
file (GLOB SOURCES "*.cc")

add_executable(meshconvert ${SOURCES} ${HEADERS})
target_link_libraries(meshconvert PRIVATE mve mve_util)
install(TARGETS meshconvert RUNTIME DESTINATION .)
