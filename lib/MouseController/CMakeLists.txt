set(LIB_NAME MouseController)

add_library(${LIB_NAME} mouse_controller.cpp)

target_include_directories(
  ${LIB_NAME}
  INTERFACE ${CMAKE_CURRENT_SOURCE_DIR}
)

target_link_libraries(
  ${LIB_NAME}
#  pico_stdlib
)

add_dependencies(
  ${LIB_NAME}
#  pico_stdlib
)

install(TARGETS ${LIB_NAME} DESTINATION lib)