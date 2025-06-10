# tfj - Terraform Fuzzy Jump

A zsh function that provides fuzzy directory navigation for Terraform projects within a git repository.

## Overview

`tfj` (Terraform Fuzzy Jump) allows you to quickly navigate to Terraform directories in your git repository using fuzzy search. It searches for directories containing `.terraform/terraform.tfstate` files and presents them in an interactive fuzzy finder interface.

## Features

- Automatically detects Terraform directories by looking for `.terraform/terraform.tfstate` files
- Uses fuzzy search for quick directory selection
- Works from any subdirectory within a git repository

## Dependencies

This function requires the following external commands:

- `git` - For detecting the repository root
- `rg` (ripgrep) - For fast file searching
- `fzf` - For fuzzy selection interface

## Installation

### Manual Installation

1. Clone this repository or download the `tfj.zsh` file
2. Source the file in your `.zshrc`:

```bash
source /path/to/tfj.zsh
```

### Using zinit

Add the following to your `.zshrc`:

```bash
zinit light shmokmt/tfj
```

## Usage

```bash
tfj
```
