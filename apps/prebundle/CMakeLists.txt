file (GLOB HEADERS "*.h")
file (GLOB SOURCES "*.cc")

add_executable(prebundle ${SOURCES} ${HEADERS})
target_link_libraries(prebundle PRIVATE mve mve_sfm mve_util)
install(TARGETS prebundle RUNTIME DESTINATION .)
