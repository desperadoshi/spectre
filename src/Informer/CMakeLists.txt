# Distributed under the MIT License.
# See LICENSE.txt for details.

set(LIBRARY Informer)

set(LIBRARY_SOURCES
  Informer.cpp
  Verbosity.cpp
  ${CMAKE_BINARY_DIR}/Informer/InfoAtCompile.cpp
  )

add_spectre_library(${LIBRARY} ${LIBRARY_SOURCES})

target_link_libraries(
  ${LIBRARY}
  PUBLIC
  Boost::boost
  Options

  PRIVATE
  ErrorHandling
  )

add_subdirectory(Python)
