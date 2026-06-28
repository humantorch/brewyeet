# brewyeet

A single command to fully update, clean, and health-check your Homebrew installation.

## Install

```sh
brew tap humantorch/tap
brew install brewyeet
```

## Usage

```sh
brewyeet
```

Runs the following in sequence:

1. `brew update` — fetch latest formulae
2. `brew upgrade` — upgrade all installed formulae and casks
3. `brew autoremove` — remove orphaned dependencies
4. `brew cleanup -s --prune=all` — purge old downloads and cached files
5. `brew outdated` — list anything still outdated (e.g. pinned packages)
6. `brew doctor` — run Homebrew diagnostics
