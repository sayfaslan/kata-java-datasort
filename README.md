# Data sorting utility

`datasort` is console utility for sorting data from text files. Able to handle strings, integers and floats.
Resulting output are separate files for each data type.

## Input

Text files, which contains unsorted unordered strings, integers and floats. As delimiter for tokens in files are used newline symbol.

## Features

Writes each data type into different specific file. Default filenames - integers.txt, floats.txt, strings.txt.
Creates specific file only if there is according data; empty default file not needed. 

## Options

- `-o`: defines a path for output file (`datasort -o /some/path`). Default path - current folder.
- `-p`: adds prefix to default filename (`datasort -o /some/path -p result_`).
- `-a`: adds data into file; without this option (by default) file will be overwritten.
- `-s`: collects short statistics. Saves amount of elements for each type. Printed into console for each type.
- `-f`: collects full statistics. Additionally saves - for numbers: min, max, sum and average values;
for strings: min and max string length. Printed into console for each type.

## Exceptions

Utility handles all possible exceptions and don't crash. In case of any error, utility must inform user about it
and it's cause. Partial execution is preferred instead of stopping the utility.

## Code style

`datasort` is written with "Clean code" in mind.

### Utility specs

- language ver.: Java 21;
- building tool: Maven;
- libs: not used;
