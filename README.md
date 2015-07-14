# jam3-install-analytics

Tracking our npm installs. Only tested on UNIX shells.

This is used internally; if you are interested in something similar see [npm-install-analytics](https://github.com/mattdesl/npm-install-analytics).

## Install

```sh
npm install -g jam3-install-analytics
```

This will provide a couple of global tools.

## Setup

Once installed, you need to configure a `rc` file. Run the following:

```sh
jam3-install-analytics-setup
```

It will prompt for a username and the relevant tracking ID. Once these are set, we shouldn't change them.

## Alias

This step is optional, but recommended.

You can add the following alias to `~/.bash_profile` if you would like to alias the command:

```sh
alias npm='jam3-install-analytics'
```

Now when you re-start bash, typing `npm install` will silently send information to Google Analytics with your username. 

Other commands, like `npm view`, should be unaffected.

## License

MIT, see [LICENSE.md](http://github.com/mattdesl/npm-install-analytics/blob/master/LICENSE.md) for details.
