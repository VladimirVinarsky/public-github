# Public repository for useful bash scripts

## `remove_long_names.sh`

This script helps to remove redundant (not unique) parts of filenames

\# INFO #

* The script "$0" removes the longest shared (redundant) part of filenames supplied to the script
* After finding the common sequence you can choose if you want to remove it from the filenames
* You can decide if you want to keep a copy of files with the old filenames"
* The script accepts globbing ('*' and such)"

NOTE: Works only on files in the current directory\
NOTE: When using globbing make sure not to include the script filename

\# USAGE #

`$0 FILE1 FILE2...`\
`Longest shared sequence is: ... `\
`Do you want to remove this sequence from the filenames? [y/n]`\
`Do you want to keep the old files? [y/n]`\
`Script $0 is done`


