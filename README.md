# Getting Started with Cursor, Git, and Python

This guide will help you set up your development environment and learn the basics of using Cursor IDE with Git and Python.

## Prerequisites

Before you start, make sure you have the following tools installed:

1. **Cursor IDE**: Download and install from [cursor.sh](https://cursor.sh)
2. **Git**: For version control
3. **Python**: For development
4. **GitHub Account**: For hosting your code

## Setting Up Your Environment

### 1. Git Setup

First, you need to configure Git with your information:

```bash
git config --global user.name "Your Name"
git config --global user.email "your.email@example.com"
```

### 2. Python Environment Setup

Python projects often use virtual environments to manage dependencies. We'll use `pyproject.toml` for modern Python project management. Here's what you need to know:

- `pyproject.toml` is a configuration file that defines your project's metadata and dependencies
- It's the modern standard for Python packaging and project configuration
- It replaces older tools like `setup.py` and `requirements.txt`

### 3. GitHub Setup

1. Create a GitHub account at [github.com](https://github.com)
2. Set up SSH keys for secure authentication:
   ```bash
   ssh-keygen -t ed25519 -C "your.email@example.com"
   ```
3. Add the SSH key to your GitHub account

## Basic Workflow in Cursor

### Creating a New Project

1. Open Cursor
2. Create a new directory for your project
3. Initialize a Git repository:
   ```bash
   git init
   ```
4. Create a basic Python project structure:
   ```bash
   mkdir my_project
   cd my_project
   ```

### Setting Up Python Project

1. Create a `pyproject.toml` file:
   ```toml
   [project]
   name = "my-project"
   version = "0.1.0"
   description = "My first Python project"
   requires-python = ">=3.9"
   dependencies = [
       "requests>=2.28.0",
   ]
   ```

2. Create a virtual environment:
   ```bash
   python -m venv .venv
   source .venv/bin/activate  # On macOS/Linux
   # or
   .venv\Scripts\activate  # On Windows
   ```

### Basic Git Commands

```bash
# Check status of your files
git status

# Add files to staging
git add .

# Commit changes
git commit -m "Your commit message"

# Push to GitHub
git push origin main
```

### Using Cursor Features

1. **Command Palette**: Press `Cmd/Ctrl + Shift + P` to access all commands
2. **Git Integration**: Use the Source Control panel (Git icon) to manage your changes
3. **AI Assistance**: Use `Cmd/Ctrl + K` to get AI help with your code
4. **Terminal**: Access the integrated terminal with `Cmd/Ctrl + J`

## Best Practices

1. Always commit your changes with meaningful messages
2. Keep your virtual environment in `.gitignore`
3. Regularly pull changes from remote repositories
4. Use branches for new features or bug fixes

## Getting Help

- Cursor Documentation: [cursor.sh/docs](https://cursor.sh/docs)
- Git Documentation: [git-scm.com/doc](https://git-scm.com/doc)
- Python Documentation: [python.org/doc](https://python.org/doc)

## Next Steps

1. Create your first repository on GitHub
2. Clone it to your local machine
3. Start coding with Cursor's AI assistance
4. Commit and push your changes

Remember: Practice makes perfect! Don't hesitate to experiment with these tools and features.
