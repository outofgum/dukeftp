# dukeftp

duke FTP is a FTP client with custom features. It can be used for automatic, rule-based transferring of directories.

*duke is still in early development state. Make sure to read the changelog of newer versions when upgrading. Please report all crashes of the latest version.*

[Issue / Task tracker](https://github.com/outofgum/dukeftp/issues)

[Tasks in progress](https://github.com/outofgum/dukeftp/labels/in%20progress)

[Milestones](https://github.com/outofgum/dukeftp/milestones)

We accept Bitcoin donations to support the development of the project: 1NGUfE7zzpQo8BW4Yj3LFvWQ1Hu1PWJquK

## Features

* FTP client with [FTPS](https://en.wikipedia.org/wiki/FTPS) support
* [FXP](https://en.wikipedia.org/wiki/File_eXchange_Protocol) support for direct transfer between FTP servers
* Cross-platform: Windows XP+, Mac OS X 10.8+, Linux 2.6.23+
* Multi CPU architecture: x86, x64, ARM6/7/8 (Raspberry Pi 1/2/3)
* Static compiled binary, needs no extra installation of libraries
* Socks5 proxy support for FTP, IRC and Web access
* Database client for PostgreSQL and MySQL
* IRC client with blowfish encryption support
* Administration by IRC commands
* [TOML](https://github.com/toml-lang/toml) based configuration files that can be edited manually

## Installation
* Download a "Source code" file from [releases]( https://github.com/outofgum/dukeftp/releases) and unpack it or clone the git.
* Download a duke version that matches your system architecture from [releases]( https://github.com/outofgum/dukeftp/releases).
* Unpack duke and copy the binary to the bin folder.
* Edit the config files, at least a correct IRC config for an admin channel is needed to start duke.
* Start the duke binary. You will be asked for a password that is used to crypt and decrypt the config files.

## Milestones

You can see the remaining tasks for the milestones of the project:

- [Download bot](https://github.com/outofgum/dukeftp/milestone/2)
- [Request fill bot](https://github.com/outofgum/dukeftp/milestone/3)
- [Pre bot](https://github.com/outofgum/dukeftp/milestone/4)
- [Autotrader](https://github.com/outofgum/dukeftp/milestone/5)
