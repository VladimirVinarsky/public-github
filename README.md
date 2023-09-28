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


## `reorganize_daily_images.sh`

This script reorganizes images stored in chronologically labelled folders into image ID labelled folders while sorting
them by date.

\# INFO #
 
Usage: $0 <parent-folder>                  \
Supply path to <parent-folder> which contains multiple <sub-folders>.\
\
Each <sub-folder> contains images taken in one day.\
Example <sub-folder>: 11-10-2023.\
\
The image names start with CellLineId: #0001 - #9999 which is followed by details (objective,comment etc).\
Example image: #0003_sparse_good-morpholgy_10x.tif\
\
The script will bring together images of each CellLineId and sort them from newest to oldest\
Reorganized images will appear in 'Reorganized' folder\
\
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++\
                          >  Let's go  <                             \
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++\
\
