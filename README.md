# Shell Script Input Redirection and Word Splitting Error

This repository demonstrates a common error in shell scripting related to input redirection and word splitting.  The script `bug.sh` attempts to read lines from a file, but it fails to handle lines containing spaces or special characters correctly due to word splitting. The corrected version is provided in `bugSolution.sh`. 

## Bug Description
The original script uses a simple `while read` loop, which is susceptible to word splitting. This means that if a line in the input file contains spaces, it will be split into multiple words, leading to unexpected behavior. 

## Solution
The solution utilizes the `-d ''` option in `while read`, which allows it to properly handle lines that might contain spaces or special characters.