# Bash Scripting Cheatsheet

---

## Table of Contents

# GitHub-style Table of Contents for Bash Cheatsheet

# GitHub-style Table of Contents for Bash Cheatsheet

| Section | Description |
|---------|-------------|
| [introduction](https://github.com/ohm-vishwa/learn-from-error-res/blob/main/bash-cheat-sheet.md#1-introduction) | What is Bash, scripts, and the shell |
| [basic commands](https://github.com/ohm-vishwa/learn-from-error-res/blob/main/bash-cheat-sheet.md#2-basic-commands) | Essential file and directory commands |
| [creating & running scripts](https://github.com/ohm-vishwa/learn-from-error-res/blob/main/bash-cheat-sheet.md#3-creating--running-scripts) | How to write and execute scripts |
| [variables (all ways to declare)](https://github.com/ohm-vishwa/learn-from-error-res/blob/main/bash-cheat-sheet.md#4-variables-all-ways-to-declare) | Declaring, exporting, and using variables |
| [quoting & escaping](https://github.com/ohm-vishwa/learn-from-error-res/blob/main/bash-cheat-sheet.md#5-quoting--escaping) | Single/double quotes, escaping characters |
| [comments](https://github.com/ohm-vishwa/learn-from-error-res/blob/main/bash-cheat-sheet.md#6-comments) | Adding comments to scripts |
| [user input (all ways to read)](https://github.com/ohm-vishwa/learn-from-error-res/blob/main/bash-cheat-sheet.md#7-user-input-all-ways-to-read) | Reading input from users and files |
| [command substitution](https://github.com/ohm-vishwa/learn-from-error-res/blob/main/bash-cheat-sheet.md#8-command-substitution) | Capturing command output in variables |
| [arithmetic](https://github.com/ohm-vishwa/learn-from-error-res/blob/main/bash-cheat-sheet.md#9-arithmetic) | Performing calculations in Bash |
| [conditionals](https://github.com/ohm-vishwa/learn-from-error-res/blob/main/bash-cheat-sheet.md#10-conditionals) | if/else statements and tests |
| [case statement](https://github.com/ohm-vishwa/learn-from-error-res/blob/main/bash-cheat-sheet.md#11-case-statement) | Multi-way branching with case |
| [loops](https://github.com/ohm-vishwa/learn-from-error-res/blob/main/bash-cheat-sheet.md#12-loops) | for, while, until loops |
| [functions](https://github.com/ohm-vishwa/learn-from-error-res/blob/main/bash-cheat-sheet.md#13-functions) | Defining and using functions |
| [positional parameters & special vars](https://github.com/ohm-vishwa/learn-from-error-res/blob/main/bash-cheat-sheet.md#14-positional-parameters--special-vars) | Script arguments and special variables |
| [arrays](https://github.com/ohm-vishwa/learn-from-error-res/blob/main/bash-cheat-sheet.md#15-arrays) | Indexed and associative arrays |
| [string manipulation](https://github.com/ohm-vishwa/learn-from-error-res/blob/main/bash-cheat-sheet.md#16-string-manipulation) | Substrings, replacement, and more |
| [file & directory tests](https://github.com/ohm-vishwa/learn-from-error-res/blob/main/bash-cheat-sheet.md#17-file--directory-tests) | Checking file and directory properties |
| [redirection](https://github.com/ohm-vishwa/learn-from-error-res/blob/main/bash-cheat-sheet.md#18-redirection) | Redirecting input/output |
| [pipes & filters](https://github.com/ohm-vishwa/learn-from-error-res/blob/main/bash-cheat-sheet.md#19-pipes--filters) | Chaining commands and filtering data |
| [globbing & wildcards](https://github.com/ohm-vishwa/learn-from-error-res/blob/main/bash-cheat-sheet.md#20-globbing--wildcards) | Pattern matching with wildcards |
| [process management](https://github.com/ohm-vishwa/learn-from-error-res/blob/main/bash-cheat-sheet.md#21-process-management) | Background jobs and process control |
| [traps & signal handling](https://github.com/ohm-vishwa/learn-from-error-res/blob/main/bash-cheat-sheet.md#22-traps--signal-handling) | Handling signals and cleanup |
| [debugging](https://github.com/ohm-vishwa/learn-from-error-res/blob/main/bash-cheat-sheet.md#23-debugging) | Debugging and error tracing |
| [here documents & strings](https://github.com/ohm-vishwa/learn-from-error-res/blob/main/bash-cheat-sheet.md#24-here-documents--strings) | Multi-line input and here strings |
| [regular expressions](https://github.com/ohm-vishwa/learn-from-error-res/blob/main/bash-cheat-sheet.md#25-regular-expressions) | Pattern matching with regex |
| [associative arrays (bash 4+)](https://github.com/ohm-vishwa/learn-from-error-res/blob/main/bash-cheat-sheet.md#26-associative-arrays-bash-4) | Key-value arrays (Bash 4+) |
| [date & time](https://github.com/ohm-vishwa/learn-from-error-res/blob/main/bash-cheat-sheet.md#27-date--time) | Working with dates and times |
| [file processing](https://github.com/ohm-vishwa/learn-from-error-res/blob/main/bash-cheat-sheet.md#28-file-processing) | Reading and processing files |
| [networking](https://github.com/ohm-vishwa/learn-from-error-res/blob/main/bash-cheat-sheet.md#29-networking) | Network commands and scripting |
| [argument parsing](https://github.com/ohm-vishwa/learn-from-error-res/blob/main/bash-cheat-sheet.md#30-argument-parsing) | Handling script options and arguments |
| [scheduling & automation](https://github.com/ohm-vishwa/learn-from-error-res/blob/main/bash-cheat-sheet.md#31-scheduling--automation) | Automating tasks with cron/at |
| [advanced topics](https://github.com/ohm-vishwa/learn-from-error-res/blob/main/bash-cheat-sheet.md#32-advanced-topics) | Advanced Bash scripting features |
| [quick reference](https://github.com/ohm-vishwa/learn-from-error-res/blob/main/bash-cheat-sheet.md#33-quick-reference) | Handy Bash tips and tricks |
| [troubleshooting](https://github.com/ohm-vishwa/learn-from-error-res/blob/main/bash-cheat-sheet.md#34-troubleshooting) | Common errors and solutions |
| [resources & further reading](https://github.com/ohm-vishwa/learn-from-error-res/blob/main/bash-cheat-sheet.md#35-resources--further-reading) | Helpful links and documentation |
| [best practices](https://github.com/ohm-vishwa/learn-from-error-res/blob/main/bash-cheat-sheet.md#36-best-practices) | Writing clean, safe scripts | 
---

## 1. Introduction
- **Bash**: Bourne Again SHell, a command-line interpreter.
- **Script**: Text file with commands, usually ending in `.sh`.
- **Shebang**: First line in script: `#!/bin/bash`

---

## 2. Basic Commands
- `ls` – List files
- `cd dir` – Change directory
- `pwd` – Print working directory
- `cp src dest` – Copy files
- `mv src dest` – Move/rename files
- `rm file` – Remove file
- `mkdir dir` – Make directory
- `rmdir dir` – Remove directory
- `touch file` – Create empty file
- `cat file` – Show file contents
- `echo text` – Print text

---

## 3. Creating & Running Scripts
```bash
#!/bin/bash
# Save as script.sh
chmod +x script.sh   # Make executable
./script.sh          # Run script
```

---

## 4. Variables (All Ways to Declare)

### Basic Variable Declaration
```bash
var=value
name="Alice"
```
- No spaces around `=`.
- Variable names: letters, numbers, underscores (cannot start with a number).

### Read-Only (Constant) Variable
```bash
readonly pi=3.14
# or
declare -r pi=3.14
```

### Exporting Variables (for child processes)
```bash
export PATH="$PATH:/new/path"
export MYVAR=123
```

### Declaring with `declare` or `typeset`
```bash
declare var="hello"
typeset var2=42  # Same as declare, mostly in functions
```

### Integer Variable
```bash
declare -i num=10
let num=5+3
```

### Array Variable
```bash
arr=(one two three)
declare -a arr2=(a b c)
```

### Associative Array (Bash 4+)
```bash
declare -A map
map[foo]=bar
```

### Unset (Delete) Variable
```bash
unset var
```

### Indirect Reference (Advanced)
```bash
varname="foo"
foo="bar"
echo ${!varname}  # prints 'bar'
```

---

## 5. Quoting & Escaping
- **Single quotes**: `'text'` (literal)
- **Double quotes**: `"$var"` (expands variables)
- **Escape**: `\` (e.g., `echo "A\tB"`)

---

## 6. Comments
```bash
# This is a comment
```

---

## 7. User Input (All Ways to Read)

### Using `read` (most common)
```bash
read var
read -p "Enter your name: " name
read -s secret  # Silent (no echo)
read -n 1 char  # Read one character
read -a arr     # Read into array
read -r line    # Raw input (no backslash escapes)
read -t 5 timed # Timeout after 5 seconds
read -d ":" val # Read until delimiter ':'
```

### Reading from a file (line by line)
```bash
while IFS= read -r line; do
  echo "$line"
done < file.txt
```

### Reading all input at once
```bash
input=$(cat)
# or
input="$(<file.txt)"
```

### Reading with `IFS` (Internal Field Separator)
```bash
IFS="," read -ra arr <<< "a,b,c"
```

### Using `select` for Menus
```bash
select opt in "A" "B" "C"; do
  echo "You chose $opt"
  break
done
```

---

## 8. Command Substitution
```bash
date=$(date)
echo "Today: $date"
```

---

## 9. Arithmetic
```bash
a=5; b=3
sum=$((a + b))
echo $sum
let c=a*b
echo $c
```

---

## 10. Conditionals
```bash
if [ $a -gt $b ]; then
  echo "a > b"
elif [ $a -eq $b ]; then
  echo "a == b"
else
  echo "a < b"
fi
```

---

## 11. Case Statement
```bash
case $var in
  1) echo "One";;
  2) echo "Two";;
  *) echo "Other";;
esac
```

---

## 12. Loops
```bash
for i in 1 2 3; do echo $i; done
while [ $a -gt 0 ]; do echo $a; ((a--)); done
until [ $a -eq 0 ]; do echo $a; ((a--)); done
```

---

## 13. Functions
```bash
myfunc() {
  echo "Hello $1"
}
myfunc World
```

---

## 14. Positional Parameters & Special Vars
- `$0` – Script name
- `$1`, `$2`, ... – Arguments
- `$@` – All args
- `$#` – Number of args
- `$?` – Last command exit status
- `$$` – Script PID
- `$!` – PID of last background job

---

## 15. Arrays
```bash
arr=(one two three)
echo ${arr[0]}
echo ${arr[@]}
for i in "${arr[@]}"; do echo $i; done
```

---

## 16. String Manipulation
```bash
str="abcdef"
echo ${#str}         # Length
echo ${str:2:3}      # Substring
echo ${str/abc/xyz}  # Replace
```

---

## 17. File & Directory Tests
```bash
[ -e file ]   # Exists
[ -f file ]   # Regular file
[ -d dir ]    # Directory
[ -r file ]   # Readable
[ -w file ]   # Writable
[ -x file ]   # Executable
```

---

## 18. Redirection
- `>` – stdout to file (overwrite)
- `>>` – stdout to file (append)
- `<` – stdin from file
- `2>` – stderr to file
- `&>` – stdout+stderr to file
- `tee` – output to file and screen

---

## 19. Pipes & Filters
```bash
cat file | grep "pattern" | sort | uniq
```
Common filters: `grep`, `awk`, `sed`, `cut`, `tr`, `sort`, `uniq`, `head`, `tail`

---

## 20. Globbing & Wildcards
- `*` – Any chars
- `?` – Single char
- `[abc]` – a, b, or c
- `{a,b}` – a or b

---

## 21. Process Management
- `command &` – Run in background
- `jobs` – List jobs
- `ps` – List processes
- `kill PID` – Kill process
- `wait` – Wait for background jobs
- `fg`, `bg` – Foreground/background

---

## 22. Traps & Signal Handling
```bash
trap "echo Exiting!" SIGINT SIGTERM
```

---

## 23. Debugging
- `set -x` – Debug mode (trace)
- `set -e` – Exit on error
- `bash -n script.sh` – Syntax check
- `bash -v script.sh` – Verbose

---

## 24. Here Documents & Strings
```bash
cat <<EOF
multi-line
text
EOF
cat <<< "one line"
```

---

## 25. Regular Expressions
```bash
echo "abc" | grep -E "^a.*c$"
[[ "abc" =~ ^a.*c$ ]] && echo "match"
```

---

## 26. Associative Arrays (Bash 4+)
```bash
declare -A map
map[foo]=bar
echo ${map[foo]}
for k in "${!map[@]}"; do echo $k; done
```

---

## 27. Date & Time
```bash
date
now=$(date +%s)
```

---

## 28. File Processing
```bash
while IFS= read -r line; do echo $line; done < file.txt
```

---

## 29. Networking
- `curl`, `wget` – Download files
- `nc` – Netcat for networking

---

## 30. Argument Parsing
```bash
while getopts "a:b:" opt; do
  case $opt in
    a) aval=$OPTARG;;
    b) bval=$OPTARG;;
  esac
done
```

---

## 31. Scheduling & Automation
- `crontab -e` – Edit cron jobs
- `at 10:00` – Run at specific time

---

## 32. Advanced Topics
- **Command Substitution**: `$(...)` vs `` `...` ``
- **Here Documents**: `<<< "string"` vs `<<EOF`
- **Arrays**: Indexed vs Associative
- **String Manipulation**: Substring, Replacement, Length
- **File Tests**: `-e`, `-f`, `-d`, `-r`, `-w`, `-x`
- **Redirection**: `>`, `>>`, `<`, `2>`, `&>`, `tee`
- **Pipes & Filters**: Chaining, Filtering, Sorting
- **Globbing**: `*`, `?`, `[abc]`, `{a,b}`
- **Process Management**: `&`, `jobs`, `ps`, `kill`, `wait`, `fg`, `bg`
- **Traps & Signal Handling**: `trap`, `SIGINT`, `SIGTERM`
- **Debugging**: `set -x`, `set -e`, `bash -n`, `bash -v`
- **Here Documents & Strings**: `<<EOF`, `<<< "string"`
- **Regular Expressions**: `grep -E`, `[[ =~ ]]`
- **Associative Arrays**: `declare -A`, `map[key]=value`
- **Date & Time**: `date`, `now=$(date +%s)`
- **File Processing**: `while IFS= read -r line; do ... done`
- **Networking**: `curl`, `wget`, `nc`
- **Argument Parsing**: `while getopts "a:b:" opt; do ... done`
- **Scheduling & Automation**: `crontab -e`, `at 10:00`

---

## 33. Quick Reference
- `!!` – Repeat last command
- `!$` – Last argument of previous command
- `Ctrl+R` – Reverse search history
- `cd -` – Switch to previous directory
- `pushd`/`popd` – Directory stack navigation
- `history` – Show command history
- `alias ll='ls -l'` – Create command alias
- `set -x` – Enable debug mode
- `set +x` – Disable debug mode
- `: > file` – Truncate file (empty it)
- `true`/`false` – Always succeed/fail
- `command` – Run command, ignoring shell function/alias
- `type cmd` – Show how command will be interpreted

---

## 34. Troubleshooting
- **Check exit status:** `echo $?`
- **Syntax errors:** Use `bash -n script.sh` to check for syntax errors
- **Debugging:** Use `set -x` to trace execution
- **Unset variables:** Use `set -u` to error on unset variables
- **Check permissions:** Ensure scripts are executable (`chmod +x script.sh`)
- **Path issues:** Use `echo $PATH` to check command search path
- **File not found:** Check for typos and correct file paths
- **Infinite loops:** Use `Ctrl+C` to interrupt
- **Script not running as expected:** Add `echo` statements to print variable values
- **Check shebang:** Ensure the first line is `#!/bin/bash` or correct shell

---

## 35. Resources & Further Reading
- [GNU Bash Manual](https://www.gnu.org/software/bash/manual/bash.html)
- [Bash Guide for Beginners](https://tldp.org/LDP/Bash-Beginners-Guide/html/)
- [Advanced Bash-Scripting Guide](https://tldp.org/LDP/abs/html/)
- [ShellCheck](https://www.shellcheck.net/) – Shell script linter
- [explainshell.com](https://explainshell.com/) – Explains shell commands
- [Bash Hackers Wiki](https://wiki.bash-hackers.org/)
- [SS64 Bash Reference](https://ss64.com/bash/)
- [Awesome Bash](https://github.com/awesome-lists/awesome-bash)

---

## 36. Best Practices
- Use `#!/bin/bash` at the top of scripts
- Quote variables: `"$var"` to prevent word splitting
- Use functions to organize code and avoid repetition
- Comment your code for clarity
- Check exit codes after critical commands
- Use `set -euo pipefail` for safer scripts
- Avoid using `eval` unless absolutely necessary
- Prefer `$(...)` over backticks for command substitution
- Use meaningful variable and function names
- Handle errors gracefully and provide helpful messages
- Test scripts with different inputs and edge cases
- Keep scripts portable and avoid unnecessary dependencies 
