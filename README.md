glrnvim
=======
[![Build Status](https://travis-ci.com/beeender/glrnvim.svg?branch=master)](https://travis-ci.com/beeender/glrnvim)

A GPU-accelerated neovim GUI.


glrnvim is the fastest neovim gui in existence. Using the GPU for rendering enables optimizations that simply aren't possible without it.

See the speed from the screenshot:
![screenshot](screenshot/very_fast.gif)

## About

glrnvim combines Open**GL**, **R**ust and **N**eo**VIM** together, to make the fastest, simplest neovim GUI.

## Requisites

* [alacritty](https://github.com/jwilm/alacritty)
* [neovim](https://neovim.io)

## Installation

### Arch Linux

Install `glrnvim` from the AUR.

### Debian/Ubuntu

- Install [alacritty](https://github.com/jwilm/alacritty) and [neovim](https://neovim.io) to your system.

- Install [cargo-deb](https://github.com/mmstick/cargo-deb).

```
cargo install cargo-deb
```

- Build and install the `deb` package system-wide.

```
cargo deb --install
```

## Build

### Linux & macOS

```sh
cargo build
```

## Windows

Not difficult, just try.

## Configuration

glrnvim comes with a very flexible configuration ability, just copy [glrnvim.yml](https://github.com/beeender/glrnvim/blob/master/glrnvim.yml) to `$HOME/.config` (for Linux) or `$HOME/Library/Preferences` (for macOS) and modify it.

Please refer to [this](https://github.com/jwilm/alacritty/wiki/Changing-the-default-font) for more information about setting font.

## Tips

### Set `glrnvim` as the git editor for commit message

```sh
git config --global core.editor "glrnvim --nofork"
```


## Roadmap

* Make a rendering benchmark vim plugin to prove this is the fastest neovim GUI.
