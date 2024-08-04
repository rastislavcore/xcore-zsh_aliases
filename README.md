
# XCORE Zsh Aliases

> For wealth and prosperity of the population.

## Requirements

### OS

- Linux
  - Ubuntu
- macOS
  - Catalina
  - Big Sur
  - Sonoma

### Applications

- [Zsh](https://www.zsh.org/)
- [git](https://git-scm.com/download/linux) (optional)
- [Oh My Zsh](https://ohmyz.sh/) (optional)
- [Tor](https://www.torproject.org) (optional)
- [TorGhostNG](https://github.com/GitHackTools/TorghostNG) (optional)
- [Privoxy](https://www.privoxy.org) (good to have with Tor)

## Installation

### Add aliases (skip if added)

> Add aliases link to `.zshrc` file.

```sh
sudo nano ~/.zshrc
```

> Add the following instructions at the end of the file.

```sh
if [ -f ~/.zsh_aliases ]; then
  . ~/.zsh_aliases
fi
```

### Run command

> Please, make attention that your current `~/.zsh_aliases` will be modified.

### Linux

Using Wget:

```sh
wget https://raw.githubusercontent.com/raisty/xcore-zsh_aliases/master/.zsh_aliases-linux -nc --no-dns-cache -O ->> ~/.zsh_aliases
```

or cURL:

```sh
curl -sS https://raw.githubusercontent.com/raisty/xcore-zsh_aliases/master/.zsh_aliases-linux >> ~/.zsh_aliases
```

### macOS

Using Wget:

```sh
wget https://raw.githubusercontent.com/raisty/xcore-zsh_aliases/master/.zsh_aliases-darwin -nc --no-dns-cache -O ->> ~/.zsh_aliases
```

or cURL:

```sh
curl -sS https://raw.githubusercontent.com/raisty/xcore-zsh_aliases/master/.zsh_aliases-darwin >> ~/.zsh_aliases
```

## Contribution

Feel free to distribute, copy, contribute, comment, change the content. Fork and comments welcome.

## Disclaimer

Use at your own risk. This tool can modify your `.zsh_aliases` file. Backup is recommended.

## Privoxy

> Privoxy is a non-caching web proxy with advanced filtering capabilities for enhancing privacy, modifying web page data and HTTP headers, controlling access, and removing ads and other obnoxious Internet junk. Privoxy has a flexible configuration and can be customized to suit individual needs and tastes. It has applications for both stand-alone systems and multi-user networks.

Config for your computer proxy:

`Socks Host: localhost 9050`

## License

[WTFPL](LICENSE)
