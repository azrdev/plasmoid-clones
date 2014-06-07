project(az-lockout)

find_package(KDE4 REQUIRED)

include(KDE4Defaults)

install(DIRECTORY contents
        DESTINATION ${PLASMA_DATA_INSTALL_DIR}/plasmoids/lockout)
install(FILES metadata.desktop
        DESTINATION ${PLASMA_DATA_INSTALL_DIR}/plasmoids/lockout)

install(FILES metadata.desktop
        DESTINATION ${SERVICES_INSTALL_DIR}
        RENAME plasma-applet-lockout.desktop)

