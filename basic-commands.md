# Command Line Cheat Sheet

- `pwd` - Show the current path.

- `ls` - List all folders and files inside the current path.
  - `ls -l` - Detailed list.
  - `ls -la` - Detailed list including hidden files.

- `cd x` - Enter the 'x' directory.
  - `cd ..` - Move back one directory.
  - `cd ../..` - Move back two directories, and so on.

- `mkdir x` - Create a directory named 'x'.

- `touch x` - Create a file named 'x' inside the current directory.
  - `touch .x` - Create a hidden file named 'x'.

- `echo x` - Print 'x'.
  - `echo x > file` - Write 'x' inside the file.
  - `echo y >> file` - Append 'y' to the file, placing it above 'x' without overwriting it.

- `cat file` - View the content of the file.
  - `tac file` - View the file in reverse order.

- `rm file` - Remove the file.
  - `rm -rf dir` - Forcefully remove a non-empty directory.

- `cp file file2` - Copy 'file' to a new file named 'file2'.

- `mv file ../` - Move the file to the '../' path.

- `head file` - Show the first 5 lines of the file.
  - `head -n1 file` - Show only the first line.

- `tail` - Similar to `head` but with the last 5 lines.
  - `tail -n1 file` - Show the last line.
  - `tail -f file` - Observe real-time changes made to the file.
