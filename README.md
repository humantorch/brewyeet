# brewyeet

You know you should run `brew update && brew upgrade && brew autoremove && brew cleanup && brew doctor` regularly. You never do, because it's annoying to type and you always forget the full sequence.

`brewyeet` does all of it in one command.

## Install

```sh
brew tap humantorch/tap && brew install brewyeet
```

## Usage

```sh
brewyeet
```

Runs the full maintenance sequence in order:

1. `brew update` — fetch latest formulae
2. `brew upgrade` — upgrade all installed formulae and casks
3. `brew autoremove` — remove orphaned dependencies
4. `brew cleanup -s --prune=all` — purge old downloads and cached files
5. `brew outdated` — list anything still outdated (e.g. pinned packages)
6. `brew doctor` — run Homebrew diagnostics

One yeet to rule them all.
