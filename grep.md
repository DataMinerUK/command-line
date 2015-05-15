GREP
====

The `grep` command searches the contents of files or standard input. Regular expressions can be used. Each input line that matches at least one of the patterns is written to the standard output.

Switch options include:

* `-c` to give a count of the matched lines
* `-i` to ignore case sensitivity
* `-n` to give the line count witht the resulting output
* `-r` to search recursively

Examples
--------

* Search for a string in all txt files in subdirectories
`grep -r --include='*.txt' 'string' .`
* Search for string in text files in a single directory and ignore case
`grep -ri 'string' *.txt`
* Give only the file names as a result
`grep -ril 'string' *.txt`
* Count the files in which the string appears
`grep -ril 'string' *.txt | wc -l`

