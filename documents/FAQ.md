# FAQ

## Why dukeftp? Why not ____?

The other available tools like pftp, Preee or slftp are buggy, unstable, slow, outdated, Windows only or missing functionality. Duke is here to kick ass and chew bubble gum.

## I double-click on the exe, it asks for a password and then the window just closes.

Follow the installation instructions in the README. [Start duke from cmd.exe and not by double-clicking to see an error message.](http://superuser.com/questions/876933/running-exe-in-command-prompt)

## Where is the source code?

The main app is not open source. The config files, unit test fixtures and webinterface are open source.

## I have a "handshake failure" when connecting to a site

Duke has no [support](https://github.com/golang/go/issues/7758) for DHE-RSA SSL/TLS ciphers. Connecting to a server that only supports these outdated ciphers will result in an "handshake failure" error.
