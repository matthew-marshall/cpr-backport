cmake_minimum_required(VERSION 3.10)

add_library(cpr
    auth.cpp
    bearer.cpp
    cookies.cpp
    cprtypes.cpp
    curl_container.cpp
    curlholder.cpp
    error.cpp
    multipart.cpp
    parameters.cpp
    payload.cpp
    proxies.cpp
    proxyauth.cpp
    session.cpp
    timeout.cpp
    unix_socket.cpp
    util.cpp
    response.cpp
    redirect.cpp)

# Set version for shared libraries.
set_target_properties(cpr
     PROPERTIES
     VERSION ${${PROJECT_NAME}_VERSION}
     SOVERSION ${${PROJECT_NAME}_VERSION_MAJOR})

