set(COCOS2DX_DIR "${CMAKE_CURRENT_LIST_DIR}/example/cocos2dx")
set(DEPS_DIR "${CMAKE_CURRENT_LIST_DIR}/dependencies")
if (NOT EXISTS ${COCOS2DX_DIR})
	message("Downloading cocos2dx, this may take some time!")
	file(DOWNLOAD "http://www.cocos2d-x.org/filedown/start/334" "${DEPS_DIR}/cocos2dx.zip")
	execute_process(
		COMMAND ${CMAKE_COMMAND} -E tar x  ${DEPS_DIR}/cocos2dx.zip
		WORKING_DIRECTORY ${DEPS_DIR}
    )
endif()