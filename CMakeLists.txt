cmake_minimum_required (VERSION 3.16.0)
project (kwin-effects-appear1)

include (FeatureSummary)

set (CMAKE_CXX_STANDARD 14)
set (CMAKE_CXX_STANDARD_REQUIRED ON)
set (CMAKE_CXX_EXTENSIONS OFF)

find_package (ECM REQUIRED NO_MODULE)
set (CMAKE_MODULE_PATH
    ${CMAKE_MODULE_PATH}
    ${ECM_MODULE_PATH}
    ${ECM_KDE_MODULE_DIR}
    ${CMAKE_SOURCE_DIR}/cmake
    ${CMAKE_SOURCE_DIR}/cmake/Modules
)

include(KDEInstallDirs)
include(KDECMakeSettings)

add_subdirectory (src)

feature_summary (WHAT ALL)
