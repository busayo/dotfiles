# Forked from Simon's dotfiles which was also Forked from Paul Irish.

Fork at your discretion to continue the forking process. 

## Installation

### Using Git and the bootstrap script

- `git clone https://github.com/busayo/dotfiles.git ~/.dotfiles`
- `cd ~/.dotfiles`
- `script/bootstrap`

The install script will symlink the appropriate files in `.dotfiles` to your
home directory. Everything is configured and tweaked within `~/.dotfiles`,
though. All files and folders ending in `.symlink` get, you guessed it,
symlinked. For example: `~/.dotfiles/vim/vimrc.symlink` gets symlinked to
`~/.vimrc`.

### Git-free install

To install these dotfiles without Git:

```bash
curl -#L https://github.com/busayo/dotfiles/tarball/master | tar -xzv --strip-components 
```

### Install Homebrew formulae

When setting up a new Mac, you may want to install some common [Homebrew](http://brew.sh/) formulae (after installing Homebrew, of course):

```bash
brew bundle .brewfile
```

