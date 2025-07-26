# Go Shell

[![Go](https://img.shields.io/badge/Go-1.21%2B-blue.svg)](https://golang.org/)
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)

A minimalistic UNIX shell implementation in Go. Execute system commands, navigate directories, and experience the fundamentals of shell programming with clean, readable code.

---

## Table of Contents

- [Overview](#overview)
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Commands](#commands)
- [Project Structure](#project-structure)
- [Roadmap](#roadmap)
- [Contributing](#contributing)
- [License](#license)
- [Author](#author)

---

## Overview

**Go Shell** is a simple yet functional shell interpreter that demonstrates core Unix shell concepts. Built as a learning project to understand how shells parse commands, manage processes, and interact with the operating system through Go's standard library.

---

## Features

- Execute any system command with arguments
- Built-in `cd` command with home directory support
- Built-in `exit` command for graceful termination
- Interactive command loop with proper error handling
- Lightweight with minimal dependencies

---

## Installation

1. **Clone the repository:**
   ```bash
   git clone https://github.com/0x-4b/go-shell.git
   cd go-shell
   ```

2. **Run the shell:**
   ```bash
   go run main.go
   ```

---

## Usage

1. **Start the shell:**
   ```bash
   go run main.go
   ```

2. **Example session:**
   ```
   > ls -la
   > cd /home/user
   > pwd
   > echo "Hello, World!"
   > exit
   ```

---

## Commands

### Built-in Commands
| Command | Description |
|---------|-------------|
| `cd [path]` | Change directory (defaults to home directory) |
| `exit` | Exit the shell |

### External Commands
Any system command available in your `$PATH`:
- `ls`, `cat`, `grep`, `find`, etc.
- Commands with arguments work as expected

---

## Project Structure

```
go-shell/
├── main.go                # Main shell logic and entry point
├── go.mod                # Go module definition
├── .gitignore            # Git ignore rules
├── README.md             # This file
└── LICENSE               # MIT License
```

---

## Roadmap

- [ ] Add environment variable expansion (`$HOME`, `$PATH`)
- [ ] Implement command history with arrow key navigation
- [ ] Add tab completion for files and commands
- [ ] Support pipes and redirection (`ls | grep txt`)
- [ ] Add background process support (`command &`)
- [ ] Improve prompt with current directory display
- [ ] Add signal handling for better Ctrl+C behavior

---

## Contributing

Pull requests and suggestions are welcome!  
To contribute:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/your-feature`)
3. Commit your changes (`git commit -am 'Add new feature'`)
4. Push to the branch (`git push origin feature/your-feature`)
5. Open a Pull Request

---

## License

This project is licensed under the [MIT License](LICENSE).

---

## Author

**0x-4b**  
GitHub: [@0x-4b](https://github.com/0x-4b)

---
