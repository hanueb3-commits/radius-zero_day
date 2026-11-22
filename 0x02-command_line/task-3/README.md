# Task 3: Finding Files & Searching File Contents

## Purpose of find
`find` locates files and directories by name, type, or location. For example, `find practice/search-lab -type f -name "*.txt"` lists all text files in the workspace.

## Purpose of grep
`grep` searches for words or patterns inside files and prints the matching lines. Useful options: `-n` shows line numbers, `-i` ignores upper/lower case, `-R` searches recursively through folders.

## Finding a filename vs searching inside a file
`find` looks at file names, types, and locations. It does not read the file contents. `grep` reads the contents of files and shows which lines contain a word. I can combine them to search only certain files.

## Commands practised
- `mkdir -p practice/search-lab/docs practice/search-lab/logs`
- `find practice/search-lab -type f`
- `find practice/search-lab -type f -name "*.txt"`
- `find practice/search-lab -type d`
- `grep -n "JavaScript" practice/search-lab/docs/frontend.txt`
- `grep -in "radius" practice/search-lab/logs/development.txt`
- `grep -Rni "Git" practice/search-lab/`
- `grep -Rni "web" practice/search-lab/`
- `find practice/search-lab -type f -name "*.txt" -exec grep -n "JavaScript" {} +`
- `grep -Rni "Radius" practice/search-lab/ | tee task-3/search-results.txt`
- `cat task-3/search-results.txt`

## What I learned
I learned how to locate files with find, search file contents with grep, combine the two commands, and save command output to a file.
