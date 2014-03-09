add_executable(badvpn-udpgw
    udpgw.c
)
target_link_libraries(badvpn-udpgw system flow flowextra)
if (CMAKE_SYSTEM_NAME MATCHES "Darwin")
    target_link_libraries(badvpn-udpgw resolv)
endif ()

install(
    TARGETS badvpn-udpgw
    RUNTIME DESTINATION bin
)
