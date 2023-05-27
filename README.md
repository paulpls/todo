# To-Do List Automator
Author: [paulpls](https://github.com/paulpls)  
License: [FSF](LICENSE.md)



## About
Use this utility to automatically generate a to-do list by searching for patterns in the provided file paths. In return, you'll get a nicely formatted markdown file with direct links to your code, enabling you to pick up right where you left off.



## Dependencies
- python 3.6+
- grep (from GNU Coreutils)
- rm (from GNU Coreutils)



## Instructions
- Copy `todo.py` to your project's top-level directory (or elsewhere if you're feeling brave)
- Edit the file to customize the output:
  * `paths`: List of file paths to search (allows `*` globs) 
  * `patterns`: List of search keyords
  * `header`: Output file header
  * `outpath`: Output file path



