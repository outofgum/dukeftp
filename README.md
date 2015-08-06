####**dukeftp**

duke FTP is a FTP client with some custom features. It can be used for automatic transfering of directories based on rules.

Features:
* FTP client with AUTH SSL/TLS support
* Socks5 proxy support
* Cross-platform (Windows XP+, Mac OS X 10.6+, Linux 2.6.23+) and written in [Golang](https://golang.org/)
* [TOML](https://github.com/toml-lang/toml) based config files
* IRC client with blowfish support
* Administration by IRC commands

Special use features:
* Fast section detection for releases that comes out without need for regular expressions

Planned features:
* Web GUI for administration

Configuration files:
* group.ini - Known groups for each section
* language_audio.ini - Language tags for audio and mvid
* language_general.ini - Language tags for all other sections
* logging.ini - Logging settings for duke
* section.ini - Settings for the section detector of release names
