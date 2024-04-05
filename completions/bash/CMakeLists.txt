set(BASH_COMPLETION_DIR "${CMAKE_INSTALL_FULL_DATADIR}/bash-completion/completions")

configure_file(adb.in adb)
configure_file(fastboot.in fastboot)

if (FALSE)  # ======================== CUT ==========================
install(FILES
	"${CMAKE_CURRENT_BINARY_DIR}/adb"
	"${CMAKE_CURRENT_BINARY_DIR}/fastboot"
	DESTINATION "${BASH_COMPLETION_DIR}")
endif()  # ======================== CUT ==========================
