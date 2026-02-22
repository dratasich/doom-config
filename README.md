# doom-config

My personal emacs doom configuration.


## Installation

### Doom

- Clone repo into .config/emacs
- Symlink .emacs.d/ to .config/emacs:
  `ln -s ~/.config/emacs/ .emacs.d`

emacs/doom config is in .config/doom (see setup below)

### OS-Packages

- ripgrep
- fd-find
- fonts-symbola

Run `doom doctor` and follow instructions.

### This Config

```bash
git clone <this-repo>
ln -s <repo-path> ~/.config/doom
```


## Getting-Started

See `.config/doom/`

- `init.el`: doom packages included
- `config.el`: (emacs/package) configuration (e.g., maximize window)
- `packages.el`: extra packages (e.g. tldr)

On changes run `doom sync`
or `SPC h r r` to restart emacs. 


## Commands

- restart emacs: `SPC h r r`
- open file: `SPC f f`
- treemacs: `SPC o p`
- rotate through buffers: `C-x right`
- select buffer: `SPC b b`
- magit: `SPC g g` (`Z Z` to commit message)


## Tweaks

- restart treemacs when switching projects `SPC o p`


## Didn't work / TODO

- editorconfig
- eglot
