cmake_minimum_required(VERSION 3.0)

set(CMAKE_CXX_STANDARD 11)

include(cmake/HunterGate.cmake)

HunterGate(
    URL "https://github.com/n0k8t/hunter/archive/v0.19.137.1.tar.gz"
    SHA1 "f411b045dd72a16eb4cd9ff10abe59a49526f490"
)
project(cget)

hunter_add_package(CURL)
find_package(CURL CONFIG REQUIRED)
add_executable(cget ${CMAKE_CURRENT_SOURCE_DIR}/cget.cpp)
target_link_libraries(cget CURL::libcurl)
install(TARGETS cget RUNTIME DESTINATION bin)
