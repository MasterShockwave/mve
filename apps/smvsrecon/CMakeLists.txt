file (GLOB HEADERS "*.h")
file (GLOB SOURCES "*.cc")

add_executable(smvsrecon ${SOURCES} ${HEADERS})
target_link_libraries(smvsrecon PRIVATE mve mve_sfm mve_util)
install(TARGETS smvsrecon RUNTIME DESTINATION .)
