# XCORE Zsh Aliases

> For wealth and prosperity of the population.

A small, portable set of Zsh aliases and functions for macOS and Linux with a simple built-in UI (`xhelp`, `hello`) and consistent `--flags` support across most commands.

No extra frameworks required. It uses tools typically available on macOS and Linux and degrades gracefully if something is missing.

## Requirements

### OS

- Linux (tested on Ubuntu)
- macOS  
  - Catalina  
  - Big Sur  
  - Sonoma  
  - Tahoe  

### Shell

- Zsh (https://www.zsh.org/)

### Optional Tools (features degrade gracefully)

- git — required only for `gitk`
- Oh My Zsh — optional
- Tor — required only for `tor*` commands
- Privoxy — recommended if using Tor for HTTP/HTTPS proxying
- curl — used by `wanip` and `tor*` (usually preinstalled)
- dig — used by `wanip --dns` (optional)

## Installation

### 1) Source `~/.zsh_aliases` from `~/.zshrc`

Edit your `~/.zshrc`:

```sh
nano ~/.zshrc
```

Add this at the end:

```sh
if [ -f "$HOME/.zsh_aliases" ]; then
	. "$HOME/.zsh_aliases"
fi
```

Reload Zsh:

```sh
exec zsh -l
```

### 2) Install aliases file

⚠️ This appends to your existing `~/.zsh_aliases`. Backup is recommended.

Backup first:

```sh
cp -a ~/.zsh_aliases ~/.zsh_aliases.bak 2>/dev/null || true
```

### Linux (append)

Using cURL:

```sh
curl -fsSL https://raw.githubusercontent.com/raisty/xcore-zsh_aliases/master/.zsh_aliases-linux >> ~/.zsh_aliases
```

Using Wget:

```sh
wget -qO- https://raw.githubusercontent.com/raisty/xcore-zsh_aliases/master/.zsh_aliases-linux >> ~/.zsh_aliases
```

---

### macOS (append)

Using cURL:

```sh
curl -fsSL https://raw.githubusercontent.com/raisty/xcore-zsh_aliases/master/.zsh_aliases-darwin >> ~/.zsh_aliases
```

Using Wget:

```sh
wget -qO- https://raw.githubusercontent.com/raisty/xcore-zsh_aliases/master/.zsh_aliases-darwin >> ~/.zsh_aliases
```

### 3) Verify

Open a new terminal or reload:

```sh
exec zsh -l
```

Try:

```sh
xhelp
hello
```

## Features

### UI Commands

- `xhelp` — list available commands with short descriptions
- `hello` — system greeting (OS + machine info)

### File & System

- `remove [--force|-f] <paths...>` — safer rm (interactive by default)
- `ls`, `lsr` — human-readable, classified, colored listing
- `mountt` — pretty mount output
- `os [--id|--desc|--release|--all|--arch]` — OS info
- `usbdevices` — list USB devices
- `envpath` — print PATH one entry per line

### Networking

- `wanip [--dns|--http|--auto]` — show public IP
- `ports [--tcp|--udp|--all] [--filter <text>]` — show open ports
- `macs` — show MAC addresses

### Security & Crypto

- `pass [--len N] [--min N --max N] [--alnum|--full]` — password generator
- `sha256verify` / `sha512verify` — checksum verification
- `sshk` — SSH using specific key
- `sshgen` — generate ed25519 key
- `sshcopy` — copy public key to server
- `gitk` — run git with specific SSH key
- `torstart`, `torstop`, `torrenew`
- `torcheck`, `torip`

## Contribution

Feel free to distribute, copy, contribute, comment, or change the content.  
Forks and pull requests are welcome.

## Disclaimer

Use at your own risk.  
This tool modifies your `~/.zsh_aliases` file. Always keep a backup.

## Privoxy

Privoxy is a non-caching web proxy with advanced filtering capabilities for enhancing privacy, modifying web page data and HTTP headers, controlling access, and removing ads and other unwanted content.

Example SOCKS configuration (for Tor):

- SOCKS Host: `localhost`
- SOCKS Port: `9050`

## License

WTFPL
