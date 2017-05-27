**hexd** prints a human-readable hexdump of the specified files, or standard
input if omitted.  Its main distinguishing feature is the use of colours to
visually indicate which range of values an octet belongs to, aiding in
spotting patterns in binary data.

By default, *hexd* relies on 256-color SGR escape sequences.  Most terminal
emulators should support these today, but technically they're only defacto
standard.  However, you can override the formatting used with the
`HEXD_COLORS` environment variable (see manpage), or use the `-p` option for
plaintext output.

## Screenshot
![Screenshot](meta/screenshot.png "Output after being run on an ELF binary")

## License
MIT license.

## See also
* [pixd](http://github.com/FireyFly/pixd):
  like *hexd*, but visualizes the data fed to it using a 256-colour palette
  and half-block ("▀") characters.
