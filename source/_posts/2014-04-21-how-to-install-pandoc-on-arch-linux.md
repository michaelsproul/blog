---
layout: post
title: "How to install Pandoc on Arch Linux"
date: 2014-04-21 09:31:18 +1000
comments: true
categories: [Linux, Haskell, Arch Linux, Free Software]
---
I've found the best way to install Pandoc on Arch is to use the unofficial `[haskell-core]` repository. Until recently I was using an AUR package, but it is no longer being maintained, and is likely to give you trouble (it doesn't even install, because of dependency problems).

To add the `haskell-core` repository to your system, follow the instructions given at the [Arch Wiki](https://wiki.archlinux.org/index.php/Haskell_Package_Guidelines#.5Bhaskell-core.5D).

Once you have the repository set-up, installing Pandoc is as simple as:

```
$ sudo pacman -S haskell-pandoc
```

This will drag in a lot of haskell dependencies, but once you've installed them you'll have a perfectly working, upgradeable Pandoc.
