####**dukeftp**

duke FTP is an FTP client with some custom features. It can be used for automatic, rule-based transferring of directories.

Features:
* FTP client with AUTH SSL/TLS support
* FXP support for direct transfer between FTP servers
* Socks5 proxy support
* Cross-platform (Windows XP+, Mac OS X 10.6+, Linux 2.6.23+)
* [TOML](https://github.com/toml-lang/toml) based config files
* IRC client with blowfish support
* Administration by IRC commands

Special use features:
* Fast section detection for releases that come out without the need for regular expressions

Milestones:
1. Request fill bot
2. Pretool
3. Autotrader

Planned features:
* HTTP/DB access to get pretime of release
* NFO scraper
* IMDB / tvrage scraper
* Web GUI for administration

Configuration files:
* group.ini - Known groups for each section
* language_audio.ini - Language tags for audio and mvid
* language_general.ini - Language tags for all other sections
* logging.ini - Logging settings for duke
* section.ini - Settings for the section detector of release names
