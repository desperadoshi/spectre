# Distributed under the MIT License.
# See LICENSE.txt for details.

set(LIBRARY PoissonSolutions)

set(LIBRARY_SOURCES
  Lorentzian.cpp
  Moustache.cpp
  ProductOfSinusoids.cpp
  )

add_spectre_library(${LIBRARY} ${LIBRARY_SOURCES})

target_link_libraries(
  ${LIBRARY}
  PUBLIC
  DataStructures
  ErrorHandling
  Options
  Utilities
  )
