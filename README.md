# aptos-bingo
compile and run tests by running:
```
aptos move compile --skip-fetch-latest-git-deps
aptos move test
```
you sholud get:
```
Compiling, may take a little while to download git dependencies...
INCLUDING DEPENDENCY AptosFramework
INCLUDING DEPENDENCY AptosStdlib
INCLUDING DEPENDENCY MoveStdlib
BUILDING bingo
{
  "Result": [
    "0000000000000000000000000000000000000000000000000000000000001337::bingo_events",
    "0000000000000000000000000000000000000000000000000000000000001337::bingo_core"
  ]
}
```
```
INCLUDING DEPENDENCY AptosFramework
INCLUDING DEPENDENCY AptosStdlib
INCLUDING DEPENDENCY MoveStdlib
BUILDING bingo
Running Move unit tests
[ PASS    ] 0x1337::bingo_core::test_bingo
[ PASS    ] 0x1337::bingo_core::test_bingo_game_does_not_exist
[ PASS    ] 0x1337::bingo_core::test_bingo_game_has_ended
[ PASS    ] 0x1337::bingo_core::test_bingo_not_initialized
[ PASS    ] 0x1337::bingo_core::test_bingo_player_not_joined
[ PASS    ] 0x1337::bingo_core::test_bingo_player_not_won
[ PASS    ] 0x1337::bingo_core::test_cancel_game
[ PASS    ] 0x1337::bingo_core::test_cancel_game_bingo_not_initialized
[ PASS    ] 0x1337::bingo_core::test_cancel_game_does_not_exist
[ PASS    ] 0x1337::bingo_core::test_cancel_game_has_ended
[ PASS    ] 0x1337::bingo_core::test_check_columns
[ PASS    ] 0x1337::bingo_core::test_check_diagonals
[ PASS    ] 0x1337::bingo_core::test_check_player_numbers
[ PASS    ] 0x1337::bingo_core::test_check_rows
[ PASS    ] 0x1337::bingo_core::test_create_game
[ PASS    ] 0x1337::bingo_core::test_create_game_bingo_not_initialized
[ PASS    ] 0x1337::bingo_core::test_create_game_invalid_timestamp
[ PASS    ] 0x1337::bingo_core::test_create_game_name_taken
[ PASS    ] 0x1337::bingo_core::test_init
[ PASS    ] 0x1337::bingo_core::test_init_signer_not_admin
[ PASS    ] 0x1337::bingo_core::test_inser_number_game_not_started_yet
[ PASS    ] 0x1337::bingo_core::test_insert_number
[ PASS    ] 0x1337::bingo_core::test_insert_number_bingo_not_initialized
[ PASS    ] 0x1337::bingo_core::test_insert_number_duplicated
[ PASS    ] 0x1337::bingo_core::test_insert_number_game_does_not_exist
[ PASS    ] 0x1337::bingo_core::test_insert_number_invalid
[ PASS    ] 0x1337::bingo_core::test_join_game
[ PASS    ] 0x1337::bingo_core::test_join_game_already_started
[ PASS    ] 0x1337::bingo_core::test_join_game_bingo_not_initialized
[ PASS    ] 0x1337::bingo_core::test_join_game_does_not_exist
[ PASS    ] 0x1337::bingo_core::test_join_game_insufficient_funds
[ PASS    ] 0x1337::bingo_core::test_join_game_invalid_amount_of_numbers_in_column
[ PASS    ] 0x1337::bingo_core::test_join_game_invalid_number_of_columns
[ PASS    ] 0x1337::bingo_core::test_join_game_invalid_numbers_fifth_column
[ PASS    ] 0x1337::bingo_core::test_join_game_invalid_numbers_first_column
[ PASS    ] 0x1337::bingo_core::test_join_game_invalid_numbers_fourth_column
[ PASS    ] 0x1337::bingo_core::test_join_game_invalid_numbers_second_column
[ PASS    ] 0x1337::bingo_core::test_join_game_invalid_numbers_third_column
[ PASS    ] 0x1337::bingo_core::test_join_game_player_already_joined
Test result: OK. Total tests: 39; passed: 39; failed: 0
{
  "Result": "Success"
}
```
