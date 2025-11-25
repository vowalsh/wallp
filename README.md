# wallp

A beautiful, interactive wallpaper manager for macOS.

## Features

- **Interactive Browser**: Browse wallpapers with live previews using fzf
- **Gallery View**: View all wallpapers with terminal image previews
- **Smart Management**: List, filter, and organize wallpapers
- **Random Selection**: Set random wallpapers, optionally from specific folders
- **Scheduling**: Auto-rotate wallpapers at custom intervals
- **Rich CLI**: Colorful, modern terminal interface with stats and info

## Installation

1. Clone this repository
2. Make the script executable: `chmod +x wallp`
3. Add to your PATH or create a symlink:
   ```bash
   ln -s /path/to/wallp /usr/local/bin/wallp
   ```
4. Create wallpaper directory:
   ```bash
   mkdir -p ~/Desktop/wallpapers
   ```

## Quick Start

```bash
# Browse wallpapers interactively
wallp browse

# Set a random wallpaper
wallp random

# Auto-rotate every 30 minutes
wallp schedule 30m

# Show current wallpaper
wallp current
```

## Usage

```
wallp browse                   # Interactive wallpaper browser with previews
wallp gallery                  # Show gallery view of all wallpapers
wallp list [pattern]           # List all wallpapers (optional filter)
wallp set <path|number>        # Set wallpaper by path or list number
wallp random [subfolder]       # Set random wallpaper
wallp next                     # Cycle to next wallpaper
wallp prev                     # Cycle to previous wallpaper
wallp current                  # Show current wallpaper with preview
wallp info <path|number>       # Show detailed info about wallpaper
wallp schedule <interval>      # Schedule changes (e.g., 30m, 1h, 2h)
wallp schedule stop            # Stop scheduled changes
wallp schedule status          # Show schedule status
wallp folders                  # List available subfolders
wallp stats                    # Show wallpaper collection statistics
```

## Requirements

- macOS
- Bash 4.0+
- Optional: `fzf` for interactive browsing (install via `brew install fzf`)
- Optional: iTerm2, Kitty, or `timg`/`viu` for image previews

## License

MIT
