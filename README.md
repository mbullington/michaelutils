# michaelutils

Small set of Git aliases/utils.

Unlike my larger dotfiles (which are private), `michaelutils` is meant to be
lean and unassuming—I can easily clone onto SSH boxes of any UNIX system.

`michaelutils` requires:
- bash
- git
- sed
- fzf (optional)

## How to install

```sh
cd ~/.local
git clone https://github.com/mbullington/michaelutils
```

Add to `.bashrc`, `config.fish`, whatever...

```sh
export PATH="$HOME/.local/michaelutils/bin:$PATH"
```

## Utilities

- `x`: alias for `clear`

Git branching:
- `gb`: switch branches using fzf
- `gbb`: returns current branch name
- `git root`: returns git root directory

Git remote:
- `gp`: push current branch to origin
- `gpf`: push current branch to origin (with force)
- `gpp`: pull current branch from origin, after stashing, and uses --rebase strategy
- `gr`: rebase current branch off of remote `main` (or `master`)
