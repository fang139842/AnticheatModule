
AC_ADD_SCRIPT("${CMAKE_CURRENT_LIST_DIR}/src/PassiveAnticheat.cpp")
AC_ADD_SCRIPT("${CMAKE_CURRENT_LIST_DIR}/src/AnticheatMgr.cpp")
AC_ADD_SCRIPT("${CMAKE_CURRENT_LIST_DIR}/src/AnticheatScripts.cpp")
AC_ADD_SCRIPT("${CMAKE_CURRENT_LIST_DIR}/src/AnticheatData.cpp")
AC_ADD_SCRIPT("${CMAKE_CURRENT_LIST_DIR}/src/cs_anticheat.cpp")

AC_ADD_SCRIPT_LOADER("PassiveAnticheat" "${CMAKE_CURRENT_LIST_DIR}/src/loader.h")

CU_ADD_HOOK(AFTER_WORLDSERVER_CMAKE "${CMAKE_CURRENT_LIST_DIR}/src/cmake/after_ws_install.cmake")
