# Getting Started

## Installation

Download a `Source code` file from [releases](https://github.com/outofgum/dukeftp/releases) and unpack it.
The other option would bo to clone the git (which requires an installed git client):

```sh
git clone https://github.com/outofgum/dukeftp.git
```

Download a duke version that matches your system architecture from [releases](https://github.com/outofgum/dukeftp/releases).
Unpack the file and copy the binary to the bin folder of the previously downloaded `Source code`.

## Configure a proxy

If you want duke to use a SOCKS5 proxy to connect to FTP, IRC or Web, you should configure it now, otherwise skip this section.

Open `config/proxy.ini` in a text editor to configure the Proxy settings. Add a section for the proxy server and adjust them:

```ini
[moscow]
Enabled = true
User = "ohmy"
Password = "lord"
Host = "moscow.perfect-privacy.com"
Port = 5080
```

To use this proxy server for the IRC connection, you would add the following to the `default` or network section:

```ini
Proxy = "moscow"
```

## Configure an IRC admin channel to control duke

For dukeftp to work, you need to add one IRC admin channel from where you can control the tool.

Open `config/irc.ini` in a text editor to configure the IRC settings. Edit the entries of the `default` section and adjust the names:

```ini
[default]
Enabled = true
SSL = true
Nick = "mylord"
Realname = "dukeftp"
User = "mylord"
```

Those settings will be applied to all added irc networks, so you do not need to enter each of them unless they are different.

Add the IRC network where duke should connect to:

```ini
[linknet]
Host = "irc.link-net.org"
Port = 7000
SSL = true
```

Now you add a channel that uses blowfish to encrypt the communication:

```ini
[linknet.channel.mylordadmin]
Admin = true
BlowKey = "secret"
Channel = "#mylordadmin"
```

Save the file and you are ready to start duke.

## Start duke

Start the duke binary. You will be asked for a password that is used to encrypt and decrypt the config files that contain sensitive data.
Duke should connect to the configured IRC server now and join the admin channel.

## Administrate duke

The administration of duke is done by IRC commands in the admin channel. Use `!help` to see an overview of all commands.

Add your first site with the command `!addsite`. If you use a command without any parameter, the help for this command is shown.
