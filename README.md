# [bitbloxhub](https://github.com/bitbloxhub)'s flake template

A flake template that uses:

- [flake-parts](https://github.com/hercules-ci/flake-parts) to apply the NixOS module system to flakes.
- [flake-file](https://github.com/vic/flake-file) for generating `flake.nix`.
- [import-tree](https://github.com/vic/import-tree) to simplify importing files. Also has [npins](https://github.com/andir/npins) compatibility.
- [treefmt-nix](https://github.com/numtide/treefmt-nix) for formatting with `nix fmt`.
- [make-shell](https://github.com/nicknovitski/make-shell) to merge devshell definitions from multiple files with the NixOS module system.
- [flint](https://github.com/notashelf/flint) to check your flake inputs for duplicates.
- [nixfmt](https://github.com/NixOS/nixfmt), [deadnix](https://github.com/astro/deadnix), [statix](https://github.com/oppiliappan/statix), and [pedantix](https://github.com/Swarsel/pedantix) for linting and pedantic formatting your Nix code.
- [typos](https://github.com/crate-ci/typos) for spell-checking code.

## Usage

```bash
nix flake init -t github:bitbloxhub/flake-template
git init
git add .
direnv allow
```

Then put flake-parts modules in `nix/`.
