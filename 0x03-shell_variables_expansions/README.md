# 0x03. Shell, init files, variables and expansions

## Description
This project covers essential shell concepts such as:
- Creating and managing shell variables
- Understanding shell initialization files
- Performing shell arithmetic
- Using expansions, aliases, and command substitution
- Understanding reserved and environment variables

All scripts in this directory are tested on Ubuntu 20.04 LTS, contain exactly two lines, start with `#!/bin/bash`, and are executable.

---

## Scripts

### `0-alias`
Creates an alias named `ls` with the value `rm *`.  
**Warning:** Running `ls` after sourcing this script will delete all files in the current directory.

---

### `1-hello_you`
Prints `hello <current_user>`, where `<current_user>` is the username of the currently logged-in user. Uses the `$USER` variable.

---
### `2-path`
Appends `/action` to the end of the current `$PATH` environment variable.

---

### `3-paths`
Prints the number of directories currently listed in the `$PATH` variable. It includes empty fields as separate entries.  
Useful to understand how `$PATH` is parsed by the shell.

---

### `4-global_variables`
Prints all global (environment) variables currently available in the shell session using the `printenv` command.

### `5-local_variables`
Displays all local variables, environment variables, and shell functions using the `set` command.

## Usage
Make sure all scripts are executable:
```bash
chmod +x <script_name>
