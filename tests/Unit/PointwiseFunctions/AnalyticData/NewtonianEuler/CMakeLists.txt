# Distributed under the MIT License.
# See LICENSE.txt for details.

set(LIBRARY "Test_NewtonianEulerAnalyticData")

set(LIBRARY_SOURCES
  Test_KhInstability.cpp
  )

add_test_library(
  ${LIBRARY}
  "PointwiseFunctions/AnalyticData/NewtonianEuler"
  "${LIBRARY_SOURCES}"
  "NewtonianEulerAnalyticData;Options;Utilities"
  )
