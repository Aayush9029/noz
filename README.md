# noz

Prevent your Mac from sleeping when the lid is closed.

## Installation

```bash
brew install aayush9029/tap/noz
```

## Usage

```bash
noz              # Prevent sleep for 45 minutes (default)
noz -m 60        # Prevent sleep for 1 hour
noz -m 5         # Prevent sleep for 5 minutes
```

Press Enter to stop early, or wait for the timeout (which triggers sleep).

## Options

| Flag | Description |
|------|-------------|
| `-h, --help` | Show help |
| `-v, --version` | Show version |
| `-m, --minutes N` | Duration in minutes (default: 45) |

## Requirements

- macOS
- sudo access (for pmset)
