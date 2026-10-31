[![FriendsOfGo](https://img.shields.io/badge/powered%20by-Friends%20of%20Go-73D7E2.svg)](https://img.shields.io/badge/powered%20by-Friends%20of%20Go-73D7E2.svg)

# homebrew-tap

Homebrew casks for Friends of Go binaries.

Install Killgrave on macOS or Linux (Intel or ARM, 64-bit):

```sh
brew install --cask friendsofgo/tap/killgrave
```

Existing formula installations migrate to the cask through `tap_migrations.json`
when Homebrew updates and upgrades. The cask and migration mapping must be
published together with removal of `Formula/killgrave.rb`.

The initial cask uses the existing v0.5.1 release assets and checksums. Subsequent
Killgrave releases update `Casks/killgrave.rb` automatically through GoReleaser.
The unsigned macOS binary uses GoReleaser's documented quarantine-removal hook;
this bypasses Gatekeeper verification for that binary.

32-bit Linux users can download binaries from
[GitHub Releases](https://github.com/friendsofgo/killgrave/releases).
