<a href="https://nearhost.dev"><img src="https://raw.githubusercontent.com/nearhost/.github/main/assets/header-brew.png" alt="Nearhost. Run it anywhere. Open it here."></a>

# Nearhost for Homebrew

The Homebrew tap for [Nearhost](https://github.com/nearhost/nearhost), a terminal app that opens a dev server running on one of your other machines at a local `https://myapp.test`, over the SSH config you already have. You install nothing on the server, and cookies, OAuth redirects, WebSockets and hot reload behave as they do on `localhost`.

```sh
brew install nearhost/tap/nearhost
```

[Website](https://nearhost.dev) · [Docs](https://nearhost.dev/docs/getting-started/introduction/) · [Nearhost](https://github.com/nearhost/nearhost) · [Releases](https://github.com/nearhost/nearhost/releases)

![The Nearhost terminal interface: servers and projects on the left, and the selected project's address, routes and request log on the right.](https://raw.githubusercontent.com/nearhost/.github/main/assets/tui.png)

## Install and upgrade

```sh
brew install nearhost/tap/nearhost
brew upgrade nearhost
```

The cask installs the release binary for macOS or Linux, on Apple silicon, Intel or ARM. Nearhost isn't notarised, so on macOS the cask clears the quarantine flag that would otherwise stop Gatekeeper from opening it.

Then run `nearhost`. On first run it trusts its local certificate authority for you and helps you add your first project. On Linux, `nearhost doctor` prints the command that lets the binary bind ports 80 and 443; run it again after each upgrade. The [install guide](https://nearhost.dev/docs/getting-started/install/) covers the rest.

## How this tap is updated

GoReleaser writes `Casks/nearhost.rb` when Nearhost publishes a release, so don't edit it by hand. Report problems with Nearhost or the cask at [nearhost/nearhost](https://github.com/nearhost/nearhost/issues).

## Licence

MIT, like [Nearhost](https://github.com/nearhost/nearhost/blob/main/LICENSE).
