####**dukeftp**

duke FTP is a FTP client with some custom features. It can be used for automatic, rule-based transferring of directories.

Features:

* FTP client with AUTH TLS support
* FXP support for direct transfer between FTP servers
* Cross-platform: Windows XP+, Mac OS X 10.6+, Linux 2.6.23+
* Multi CPU architecture: x86, x64, ARM6+7 (Raspberry Pi 1/2)
* Static compiled binary, needs no extra installation of libraries
* Socks5 proxy support for FTP, IRC and Web access
* Built-in Socks5 proxy server
* IRC client with blowfish encryption support
* Administration by IRC commands
* [TOML](https://github.com/toml-lang/toml) based configuration files
* Written in modern programming language [Golang](https://golang.org/)
* Unit testing with high code coverage to ensure code quality

Limitations:

* No [support](https://github.com/golang/go/issues/7758) for DHE-RSA SSL/TLS ciphers. Connecting to a server that only supports these outdated ciphers will result in an "handshake failure" error.

Installation:
* Download a "Source code" file from releases and unpack it or clone the git.
* Download a duke version that matches your system from releases.
* Unpack duke and copy the binary to the bin folder.
* Edit the config files, at least an irc config for an admin channel is needed to start duke.
* Start duke binary. You will be asked for a password that is used to crypt and decrypt the config files.

Usage:

**dukeftp**
<dl>
<dt>p releasename</dt>
  <dd>Parse the release name and show extracted info. This can be used to test the section detector.</dd>
<dt>s</dt>
  <dd>Start the main application and connect to configured IRC networks. This is the default mode if no parameter is specified.</dd>
<dt>c</dt>
  <dd>Crypt the config files.</dd>
<dt>d</dt>
  <dd>Decrypt the config files.</dd>
</dl>
