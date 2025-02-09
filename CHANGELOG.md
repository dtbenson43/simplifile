# Changelog

## Unreleased

## v1.5.0 - 29 February 2024
- add `file_info` function.

## v1.4.2 - 18 February 2024
- Update msg in deprecated tag for `is_directory` to correctly point to `verify_is_directory`

## v1.4.1 - 1 February 2024
- Update gleam_stdlib dependency to "~> 0.34 or ~> 1.0" in preparation for 1.0.

## v1.3.1 - 27 January 2024
- Update msg in deprecated tag for `is_file` to correctly point to `verify_is_file`.

## v1.3.0 - 26 January 2024
- Deprecate `is_file` and `is_directory` in favor of `verify_is_file` and `verify_is_directory`,
  which error on lack of permissions rather than silently returning false.

## v1.2.0 - 11 January 2024
- Add the `current_directory` function

## v1.1.2 - 9 January 2024
- Update stdlib dep to 0.33

## v1.1.1 - 5 January 2024
- Fix bug with double "/" from `get_files`

## v1.1.0 - 25 December 2023
- Added `set_permissions` and `set_permissions_octal` functions for setting
  permissions on a file

## v1.0.0 - 16 November 2023
- No changes, just going v1 so somver starts working

## v0.4.0 - 15 November 2023
- Renamed `list_contents` to `read_directory`
- Added `get_files`

## v0.3.0 - 12 November 2023
- Switched order of parameters for `write`, `append`, `write_bits`, and `append_bits` functions.
  They now take the filename first.

## v0.2.1 - 11 November 2023
- Updated ffi js to use `BitArray`

## v0.2.0 - 6 November 2023
- Updated for Gleam v0.32.

## v0.1.14 - 18 September 2023
- added `delete_all` which takes a list of paths to call delete on

## v0.1.13 - 17 September 2023
- copy and rename directory functions perform a create_directory_all

## v0.1.12 - 17 September 2023
- Add `copy_directory` and `rename_directory` functions

## v0.1.11 - 11 September 2023
- Add `copy_file` and `rename_file` functions

## v0.1.10 - 9 August 2023
- Change `creat_dir_all` to `create_directory_all`

## v0.1.9 - 8 August 2023
- Add functions `create_dir_all`, `create_file`, and `is_file`.
- Remove function `delete_directory`. The `delete` function now deletes files
  and recursively deletes directories.
- `make_directory` is now called `create_directory` to be consistent with `create_file`.

## v0.1.8 - 31 July 2023
- Small refactor to remove js functions `writeFile` and `appendFile`

## v0.1.7 - 31 July 2023
- Fix bug where `read` was incorrectly returning non utf8 content for string on 
    javascript target. Now returns correct `NonUtf8` error

## v0.1.6 - 19 July 2023
- Add `make_directory` and `delete_directory` functions for working with directories.

## v0.1.5 - 12 July 2023
- Update to use new ffi syntax

## v0.1.4 - 21 June 2023
- Add `is_directory` and `list_contents` functions for working with directories.

## v0.1.3 - 21 June 2023
- Add ffi to remove gleam_erlang dependency

## v0.1.2 - 21 June 2023
- Remove unnecessary dependency on `gleam_javascript`. Whoops.

## v0.1.1 - 31 May 2023
- Refactored to match gleam idiom of ffi "do" functions and single signature.
- Added documentation about the utf8 issue with the read function. 
