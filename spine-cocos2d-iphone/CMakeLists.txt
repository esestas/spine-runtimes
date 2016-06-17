set(COCOS2D_DIR "${CMAKE_CURRENT_LIST_DIR}")
execute_process(COMMAND git clone --recursive https://github.com/cocos2d/cocos2d-objc cocos2d
				WORKING_DIRECTORY ${COCOS2D_DIR}) 