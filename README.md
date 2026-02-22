# doom-config

My personal emacs doom configuration.


## Installation

### Doom

Follow [doom installation instructions](https://github.com/doomemacs/doomemacs?tab=readme-ov-file#install).

Symlink .emacs.d/ to .config/emacs:
`ln -s ~/.config/emacs/ .emacs.d`

Config is in .config/doom (see setup below)

### Dependencies

Recommended OS packages:

- ripgrep
- fd-find
- fonts-symbola

Run `doom doctor` and follow instructions (e.g., for nerd icons).

Other:
```bash
# markdown +grip
go install github.com/chrishrb/go-grip@latest
```


### This Config

```bash
git clone <this-repo>
ln -s <repo-path> ~/.config/doom
```

Run `doom sync` to apply the changes.

### Daemon

To speed-up startup of emacs. Add `emacs --daemon` to autostart.


## Getting-Started

See `.config/doom/`

- `init.el`: doom packages included
- `config.el`: (emacs/package) configuration (e.g., maximize window)
- `packages.el`: extra packages (e.g. tldr)

On changes run `doom sync`
or `SPC h r r` to restart emacs. 


## Commands

| Action | Shortcut |
|--------|----------|
| restart emacs | `SPC h r r` |
| open file | `SPC f f` |
| treemacs | `SPC o p` |
| rotate through buffers | `C-x right` |
| select buffer | `SPC b b` |
| magit | `SPC g g` (`Z Z` to commit message) |


## Tweaks

- restart treemacs when switching projects `SPC o p`


## Didn't work / TODO

- editorconfig
- eglot
