# Pow Default App

Default app for use with [Pow.cx](http://pow.cx/) that lists/links your other
Pow apps.  If you have lots of Pow applications it can be hard to remember what
you've named them all.  Pow comes with [default virtual host
functionality](http://pow.cx/manual.html#section_2.1.3) which can be used with
this app to dynamically list/link your other Pow applications.

This app will try and use the first TLD configured in `POW_DOMAINS`, falling back
to `.dev`. It also works with `.xip.io` domains.

On mousever QR Codes will be displayed using your computers local IP address and xip.io.
These can then be shot with your phone to automatically load that app on your phone.

## Installation

1. Install and configure [Pow](http://pow.cx/).
1. Install and configure ImageMagick (used to generate QR Codes).
1. Download this repository and move `pow_default_app` to `$HOME/.pow/default`.
1. Configure RVM/rbenv/etc to suite your environment.
1. `bundle install`
2. Open `http://localhost.dev/` in your browser.

If everything is right, you should see a page linking to your other Pow applications.

To use with [xip.io](http://xip.io/), open `http://10.0.0.100.xip.io/` in your browser (replace 10.0.0.100 with your IP address).

**Note:** Be sure to leave `tmp/always_restart.txt` alone.  Without that file, the app will not recognize new Pow apps unless you restart Pow itself.

## Screenshots

![Example](https://raw.github.com/phallstrom/pow_default_app/master/example.png)
![Example](https://raw.github.com/phallstrom/pow_default_app/master/example-mobile.png)


## Contributions & Thanks

- [René Kersten](https://github.com/endorfin) for a much nicer UI.
- [René Kersten](https://github.com/endorfin) for QR Codes using your local IP + xip.io.
