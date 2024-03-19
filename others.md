## `grep` - Global Regular Expression Print

- `grep pattern file` - Search for a pattern in a file.
  - Example: `grep "keyword" file.txt`
  - Prints lines containing the specified pattern.

- `grep -i pattern file` - Perform a case-insensitive search.
  - Example: `grep -i "Keyword" file.txt`
  - Ignores case sensitivity when searching.

## `awk` - Pattern-Directed Scanning and Processing Language

- `awk '{print $1}' file` - Print the first field of each line.
  - Example: `awk '{print $1}' data.txt`
  - Extracts and prints the first column of data.

- `awk -F":" '{print $3}' /etc/passwd` - Set a custom field separator.
  - Example: `awk -F":" '{print $3}' /etc/passwd`
  - Uses `:` as a field separator to extract and print the third column.

## `cut` - Remove Sections from Each Line of Files

- `cut -d":" -f1 /etc/passwd` - Cut and print fields based on a delimiter.
  - Example: `cut -d":" -f1 /etc/passwd`
  - Cuts and prints the first field (column) using `:` as a delimiter.

## `sed` - Stream Editor

- `sed 's/old/new/g' file` - Replace all occurrences of "old" with "new".
  - Example: `sed 's/apples/oranges/g' fruits.txt`
  - Substitutes "apples" with "oranges" globally.

- `sed -n '1,5p' file` - Print specific lines (1 to 5).
  - Example: `sed -n '1,5p' data.txt`
  - Suppresses automatic printing and selectively prints lines 1 to 5.

## Combining Commands

- `grep "pattern" file | cut -d"," -f2` - Search and extract specific fields.
  - Example: `grep "keyword" file.txt | cut -d"," -f2`
  - Searches for a pattern and extracts the second field using `,` as a delimiter.

- `cat file.txt | grep "pattern" | sed 's/old/new/g'` - Chain commands for complex operations.
  - Example: `cat file.txt | grep "pattern" | sed 's/old/new/g'`
  - Combines commands to search, filter, and replace text.
