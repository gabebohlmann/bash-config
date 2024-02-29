# Bash-Config Custom Functions Tutorial

Enhance your terminal experience with these .bashrc functions. 
Add file select for cd with `cds`, `cd` in terminal to the `ranger` current working directory on quit with `rcd`, open file explorer in the ranger current working directory on quit with `re` and search with google in new tab in default browser with `g`.


Copy the text in bash-config.txt and paste into your .bashrc.  Update your bash config with $`. ~/.bashrc` to get started 

## Getting Started

1. Install `ranger`

`sudo apt install ranger`

2. Adding Functions to .bashrc

To use these functions, you'll need to add them to your .bashrc config file.

The .bashrc file is usually found in `~/.bashrc` (`/home/{user}/.bashrc`) 
Copy and paste the functions provided into the file.

3. Reload .bashrc 

Run

bash
$ `source ~/.bashrc`

## Function Descriptions and Usage
1. `cds`: CD with File Selector

    Purpose: Navigate through directories or open files directly from the command line, with optional support for hidden files. Uses home row first key bindings for index selection. 
    Usage:
        To use the file selector, simply type cds in your terminal.
        For including hidden files in the list, use cds -a.

2. `rcd`: Open CWD from Ranger in Terminal

    Purpose: Launch the Ranger file explorer from the current working directory (CWD) and return to the terminal in the selected directory upon exiting Ranger.
    Usage:
        Type rcd to open Ranger. Navigate to your desired directory, then quit Ranger (:q) to change your terminal's current directory to the selected one.

3. `re`: Open CWD from Ranger in Windows File Explorer

    Purpose: Similar to rcd, but opens the selected directory in Windows File Explorer, useful for WSL users.
    Usage:
        Type re to launch Ranger. Navigate and select your directory, then quit Ranger to open it in Windows File Explorer.

4. `g`: Google Search

    Purpose: Perform a Google search directly from your terminal.
    Usage:
        Type g followed by your search query. Example: g openai documentation.


Customization: Feel free to adjust the key bindings or modify the commands to fit your workflow.
Compatibility: These functions are designed for use in Bash on Linux or WSL. Ensure compatibility with your system before use.

