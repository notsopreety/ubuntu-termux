# Ubuntu-Termux

A simple, optimized script to install Ubuntu with `sudo` support in Termux on non-rooted Android devices. This sets up a lightweight Ubuntu environment where you’re logged in as root by default—no usernames or passwords needed.

## Features
- Installs Ubuntu in Termux using PRoot.
- Includes `sudo` for administrative commands.
- One-word launch command: `ubuntu`.
- Fast, reliable, and minimal setup.
- Works without root access on your device.

## Installation

Run this command in Termux to install everything in one go:

```bash
curl -sS https://raw.githubusercontent.com/notsopreety/ubuntu-termux/main/install | bash
```

This downloads and executes the script from the repo. It’ll take 2-5 minutes depending on your internet speed.

## Usage

1. After installation, start Ubuntu with:
   ```bash
   ubuntu
   ```
2. You’re logged in as root (`#` prompt).
3. Test `sudo`:
   ```bash
   sudo --version
   ```
   Or update packages:
   ```bash
   sudo apt update
   ```

## Requirements
- **Termux**: Installed from Google Play Store or F-Droid.
- **Storage**: ~1.5 GB free space.
- **Internet**: Active connection for downloading packages.

## Notes
- This is a sandboxed environment—`sudo` and root privileges are limited to Ubuntu, not your Android system.
- No user setup: You stay as root for simplicity.

## Troubleshooting
- **Fails to install?** Check your internet or storage (`df -h`).
- **Errors?** Run the curl command with `bash -x` for debug output and report it:
  ```bash
  curl -sS https://raw.githubusercontent.com/notsopreety/ubuntu-termux/main/install | bash -x
  ```

## Contributing
Feel free to fork, tweak, or submit pull requests. Issues and suggestions are welcome!

## License
MIT License—do whatever you want with it.
