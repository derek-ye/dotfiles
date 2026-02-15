# dotfiles

Nix Home Manager configurations, organized per machine. Each directory is a standalone Home Manager flake.

## Directories

- `washi-ubuntu/` — Config for **washi**, an Ubuntu machine (x86_64-linux, nixpkgs unstable). This is the current computer.
- `home-manager/` — Config for a Mac (aarch64-darwin, nixpkgs 24.11).

## Files (per directory)

- `flake.nix` — Flake inputs (nixpkgs, home-manager) and system architecture.
- `flake.lock` — Pinned dependency versions.
- `home.nix` — Packages, environment variables, and dotfile management.

## Usage

Each directory is symlinked to `~/.config/home-manager` on its respective machine, then applied with `home-manager switch`.
