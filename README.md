# 🚀 Minishell - Custom Shell Implementation

<div align="center">


</div>

## Overview
A custom implementation of a Unix shell, featuring command execution, built-in commands, and input/output redirection. This project demonstrates advanced C programming concepts including process management, signal handling, and parser implementation.


## ✨ Features

### Command Processing
- Custom command prompt display
- Command history management
- PATH-based executable location
- Relative/absolute path handling

### Quote Handling
```c
// Support for both quote types
'single quotes' // Literal interpretation
"double quotes" // Variable expansion enabled
```

### Redirections & Pipes
- Input redirection (`<`)
- Output redirection (`>`, `>>`)
- Heredoc support (`<<`)
- Multiple pipe handling (`|`)

### Built-in Commands
- `echo` with `-n` option
- `cd` with path support
- `pwd` current directory
- `export` variable management
- `unset` variable removal
- `env` environment display
- `exit` with status

## 🛠 Technical Implementation

### Signal Handling
- CTRL+C (SIGINT) management
- CTRL+D (EOF) handling
- CTRL+\ (SIGQUIT) support

### Environment Management
- Variable expansion (`$VAR`)
- Exit status access (`$?`)
- Dynamic environment updates

## 💻 Usage

### Compilation
```bash
# Build the shell
make

# Clean build files
make clean

# Full rebuild
make re
```

### Running
```bash
./minishell

minishell$ echo "Hello, $USER!"
minishell$ cd documents
minishell$ ls -l | grep ".txt" > output.txt
```


## 🔍 Key Features Demonstrated

### Parser Implementation
- Token recognition
- Command separation
- Quote handling
- Syntax validation

### Process Management
- Fork operations
- Pipe creation
- Signal handling
- Exit status management

### Memory Management
- Dynamic allocation
- Proper deallocation
- Memory leak prevention
- Resource cleanup

## 👤 Author
- group project

## 🧪 Testing
```bash
# Basic Commands
echo "Testing" > file.txt
cat < input.txt | grep "pattern" > output.txt

# Built-ins
export TEST=value
echo $TEST
cd ~/documents
```

## 📈 Project Status
- ✅ Command execution
- ✅ Built-in commands
- ✅ Redirections & pipes
- ✅ Signal handling
- ✅ Memory management



<div align="center">

*"Building robust shells from scratch"*

</div>
