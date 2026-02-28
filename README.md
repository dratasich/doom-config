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
# lsp ty for python
uv tool install ty@latest
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
| rotate through buffers | `SPC b n` or `C-x right` |
| show/select from all buffers | `SPC b B` |
| open vterm | `SPC o t` (popup) or T (here/buffer) |

### Projects

| Action | Shortcut |
|--------|----------|
| search in project | `SPC s p` |
| magit | `SPC g g` (`Z Z` to commit message) |
| compile/preview | `C-c C-c` |

### Workspace

| Action | Shortcut |
|--------|----------|
| new workspace | `SPC TAB n` |
| rename workspace | `SPC TAB n` |
| switch workspace | `SPC TAB .` or `ALT <no>` |
| select buffer (within workspace) | `SPC b b` |

### Coding

| Action | Shortcut |
|--------|----------|
| jump to definition | `SPC c d` |

Copilot:
- `copilot-login`
- Login to GitHub Enterprise, see [LSP settings](https://github.com/copilot-emacs/copilot.el?tab=readme-ov-file#lsp-settings).
  Put this into `config.el`:
  ```lisp
  (setq copilot-lsp-settings '(:github-enterprise (:uri "https://oebb.ghe.com")))
  ```


## Didn't work / TODO

- editorconfig
