# Bleep setup GitHub Action

A GitHub Action to install [bleep](https://bleep.build).

Forked from [coursier/setup-action](https://github.com/coursier/setup-action), 
which was inspired by [olafurpg/setup-scala](https://github.com/olafurpg/setup-scala) 
and the blog post [Single command Scala setup](https://alexarchambault.github.io/posts/2020-09-21-cs-setup.html) by Alex Archambault (author of Coursier).

## Features

- run bleep on any platform: Linux, MacOS, Windows
- will install the version you have configured in bleep.yaml

## Usage:

```yaml
## check out before bleep-setup-action (it relies on reading version from checked in `bleep.yaml`)
- uses: actions/checkout@v2

# add this
- uses: bleep-build/bleep-setup-action@0.0.1

## after you can just call bleep  
- run: bleep fmt --check
```