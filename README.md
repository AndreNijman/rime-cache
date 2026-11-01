# Rime binary cache

The Nix binary cache for Rime OS, served at `https://cache.rimeos.com`.

- `*.narinfo` and `nix-cache-info` are published here by Rime's release pipeline and served by GitHub Pages.
- The NAR files themselves are assets of this repository's releases; each narinfo's `URL` points at its asset.
- Every narinfo is signed with the key `rime-cache-1:LXocssi9/mdVEgEUlO+thxyiumct4b+HfqW2nIFmX1k=`. Rime machines trust
  only that key for this cache, so nothing here is trusted because of where it is hosted.

Only Rime's own builds live here (its kernel, rimed, Rime Shell, and packages the NixOS cache does not carry). Everything
else comes from `cache.nixos.org`. Nothing in this repository is edited by hand.
