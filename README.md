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
  * [paths](todo.py#L40): List of file paths to search (allows `*` globs) 
  * [patterns](todo.py#L44): List of search keyords
  * [header](todo.py#L48): Output file header
  * [outpath](todo.py#L49): Output file path
- Run the program: `python todo.py`



## Example
Given the file `example.py`:
```py
01  def do_something():
02      # TODO make this do some stuff
03  ...
```
  
With `TODO` included in the search terms, the output file will look something like this:
```markdown
# Todo List



### TODO
- [example.py](example.py#L2) make this do some stuff
...
```



