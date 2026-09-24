# homebrew-hibr

Homebrew tap for [hibr](https://github.com/osakka/hibr), a small, fast,
bash-flavoured shell.

## Install

```
brew tap osakka/hibr
brew install hibr
```

Or, to track the latest commit on `main` instead of the pinned release:

```
brew install --HEAD hibr
```

## Updating the formula

`Formula/hibr.rb` pins `url`/`sha256` to a specific commit of
[osakka/hibr](https://github.com/osakka/hibr), since the project has no
tagged releases yet. To pick up a newer commit:

```
sha=<new commit sha>
curl -sL "https://github.com/osakka/hibr/archive/$sha.tar.gz" | sha256sum
```

then update `url` and `sha256` in `Formula/hibr.rb` to match.
