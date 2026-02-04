# noz

Prevent your Mac from sleeping when the lid is closed.

## Installation

```bash
brew install Aayush9029/tap/noz
```

Or tap first:

```bash
brew tap Aayush9029/tap
brew install noz
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

## How it works

1. Disables system sleep via `pmset`
2. Runs `caffeinate` as a backup
3. Shows a live countdown timer
4. Restores original sleep settings on exit
5. Optionally triggers sleep when timeout is reached

## Requirements

- macOS
- sudo access (for pmset)

## License

MIT
