# Task 4: Bash Scripting - Automated Website Project Generator

## What the script does
`create_website.sh` automatically creates a basic website project. It makes the folders `css/`, `js/` and `images/`, and creates `index.html`, `css/style.css`, `js/script.js` and a `README.md` file in each folder. The files have real starter content, not empty files.

## How to execute it
Make it executable once, then run it:

    chmod +x task-4/create_website.sh
    ./task-4/create_website.sh

## Default output location
If no argument is given, the project is created at:

    ~/radius-projects/website-project/

## How to provide a custom output location
Give the path as the first argument. Use quotes so paths with spaces work:

    ./task-4/create_website.sh "$HOME/radius-projects/custom website"

## How the script protects existing directories
Before creating anything, the script checks if the destination already exists. If it does, it prints an error message and stops with exit code 1. It does not overwrite, modify or delete any existing files.

## Files in this directory
- `create_website.sh` - the script
- `README.md` - this file
- `screenshot.png` - terminal screenshot as evidence
