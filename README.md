# XCORE Zsh Aliases

> For wealth and prosperity of the population.

## Requirements

### OS

- Linux
   - Ubuntu
- macOS
   - Catalina
   - Big Sur

### Applications

- [Zsh](https://www.zsh.org/)
- [minio client](https://docs.min.io/docs/minio-quickstart-guide.html) (if you want use it)
- [git](https://git-scm.com/download/linux) (optional)
- [Oh My Zsh](https://ohmyz.sh/) (optional)
- [Wireguard](https://www.wireguard.com) (optional)
- [Tor](https://www.torproject.org) (optional)
- [TorGhostNG](https://github.com/GitHackTools/TorghostNG) (optional)
- [Privoxy](https://www.privoxy.org) (good to have with Tor)

## Installation

1. Add aliases (skip if added)

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

2. Run command

> Please, make attention that your current `~/.zsh_aliases` will be replaced.

> Linux

Using Wget:

```sh
wget https://raw.githubusercontent.com/raisty/xcore-zsh_aliases/master/.zsh_aliases-linux -nc --no-dns-cache -O ->> ~/.zsh_aliases
```

or cURL:

```sh
curl https://raw.githubusercontent.com/raisty/xcore-zsh_aliases/master/.zsh_aliases-linux > ~/.zsh_aliases
```

> macOS


Using Wget:

```sh
wget https://raw.githubusercontent.com/raisty/xcore-zsh_aliases/master/.zsh_aliases-darwin -nc --no-dns-cache -O ->> ~/.zsh_aliases
```

or cURL:

```sh
curl https://raw.githubusercontent.com/raisty/xcore-zsh_aliases/master/.zsh_aliases-darwin > ~/.zsh_aliases
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

## Support

Consider supporting my work with [Bitcoin][btc], [Litecoin][ltc], [Ethereum][eth], or here on [Github][gh].

[btc]: https://pay.btc.horse#bitcoin:37iSWX4QdoayZXmuj13AExuhzSkfd7LuG6
[ltc]: https://pay.btc.horse#litecoin:M8bEQNPkZ66hoFGYJuMVntyjj9dmYo1wBf
[eth]: https://pay.btc.horse#ethereum:0x10c993039CC831A1fe8230ddd82A0A13625Dd43E
[gh]: https://github.com/sponsors/raisty
