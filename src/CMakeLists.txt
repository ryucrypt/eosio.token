project(eosio.token)

find_package(cdt)

add_contract( eosio.token eosio.token eosio.token.cpp )
target_include_directories( eosio.token PUBLIC ${CMAKE_SOURCE_DIR}/../include )
target_ricardian_directory( eosio.token ${CMAKE_SOURCE_DIR}/../ricardian )