add_executable(s_chat_client chat_client.cpp)
add_executable(s_chat_server chat_server.cpp)

target_compile_options(s_chat_client PUBLIC -DASIO_STANDLONE)
target_include_directories(s_chat_client PUBLIC ${ASIO_INCLUDE_DIR})
target_link_libraries(s_chat_client PUBLIC pthread)

target_compile_options(s_chat_server PUBLIC -DASIO_STANDLONE)
target_include_directories(s_chat_server PUBLIC ${ASIO_INCLUDE_DIR})
target_link_libraries(s_chat_server PUBLIC pthread)