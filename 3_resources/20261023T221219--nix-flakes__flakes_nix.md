+++
title      = "nix flakes"
date       = 2026-10-23T22:12:19-04:00
tags       = ["flakes", "nix"]
identifier = "20261023T221219"
+++

experimental feature of nix package manager

pin versions of dependencies in a lock file

to try out flakes you first have to enable them

in nixos

`nix.settings.experimental-features = [ "nix-command" "flakes"]`

`nix flake show`
show outputs for flake
