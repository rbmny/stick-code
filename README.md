# Stick Code

An SSH-based code editor designed for iOS (specifically iPad)

## Overview

Stick Code was designed by me to solve the challenge of coding effectively from an iPad. This native iOS application provides a complete development environment by connecting to remote servers via SSH, enabling iPad users to write, edit, and manage code with the same efficiency as desktop development.

## Features

### 🔗 SSH Connection Management
- Secure SSH connections with password and public key authentication
- Connection profiles for quick access to multiple servers
- Persistent connections with automatic reconnection
- Keychain integration for secure credential storage

### 📝 Code Editing
- Syntax highlighting for multiple programming languages
- Full-featured code editor with line numbers
- File browser with directory navigation
- Multi-file editing with tabbed interface
- Search and replace functionality

### 💻 Terminal Integration
- Full terminal emulation with SSH session management
- Multiple persistent terminal sessions
- Terminal history and command completion
- Proper handling of terminal colors and formatting

### 🔄 Git Integration
- Git status and diff viewing
- Commit dialog with staged changes preview
- Branch management and repository navigation
- Visual representation of file changes

### 🎨 iPad-Optimized Interface
- Native SwiftUI design following Apple's Human Interface Guidelines
- Split-view support for multitasking
- Keyboard shortcuts and external keyboard support
- Responsive layout that adapts to different screen sizes
- Dark mode support with custom theming

## Requirements

- iOS 15.0 or later
- iPad (recommended) or iPhone
- SSH access to a remote development server

## Installation

### From Source

1. Clone this repository:
```bash
git clone https://github.com/yourusername/ssh-ide.git
cd ssh-ide
```

2. Open `ssh-ide.xcodeproj` in Xcode

3. Build and run on your iOS device or simulator

### Dependencies

The project uses the following Swift packages:
- SwiftNIO for networking
- NIOSSH for SSH protocol implementation
- SwiftData for local data persistence

## Usage

1. **Setup Connection**: Add your SSH server details including hostname, port, username, and authentication method
2. **Connect**: Tap on a connection to establish SSH session
3. **Navigate**: Use the file browser to explore your remote filesystem
4. **Edit**: Open files in the integrated code editor
5. **Terminal**: Access full terminal functionality for command-line operations
6. **Git**: View repository status and manage version control

## Architecture

The application is built using:
- **SwiftUI** for the user interface
- **SwiftData** for local data persistence
- **SwiftNIO + NIOSSH** for SSH connectivity
- **Combine** for reactive programming patterns

Key components:
- `SSHService`: Manages SSH connections and file operations
- `EditorSession`: Handles multi-file editing sessions  
- `TerminalSession`: Manages terminal emulation and command execution
- `GitService`: Provides Git integration functionality

## Contributing

This project is open source and contributions are welcome! Please feel free to:
- Report bugs and issues
- Suggest new features
- Submit pull requests
- Improve documentation

## Author

Designed and developed by **Ricardo Aguiar Bomeny** to solve the challenge of coding while being mobile

## License

This project is open source and available under the MIT License.
