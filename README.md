# Pow Default App

Default app for use with [Pow.cx](http://pow.cx/) that lists/links your other Pow apps.  If you have lots of Pow applications it can be hard to remember what you've named them all.  Pow comes with [default virtual host functionality](http://pow.cx/manual.html#section_2.1.3) which can be used with this app to dynamically list/link your other Pow applications.  

This app currently works with `.dev` domains and with `.xip.io` domains.  

## Installation

1. Install and configure [Pow](http://pow.cx/).
1. Download this repository and move it to `$HOME/.pow/default`.
1. Configure RVM/rbenv/etc to suite your environment.
1. `bundle install`
2. Open `http://localhost.dev/` in your browser.

If everything is right, you should see a page linking to your other Pow applications.

To use with [xip.io](http://xip.io/), open `http://10.0.0.100.xip.io/` in your browser (replace 10.0.0.100 with your IP address).


## Todo

- Get default TLD from Pow configuration.

## Screenshot

![Example](https://raw.github.com/phallstrom/pow_default_app/master/example.png)