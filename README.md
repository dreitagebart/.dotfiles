# Installation instructions

Clone this repo with following command:

```
git clone https://github.com/dreitagebart/.dotfiles.git ~/.dotfiles
```

Depending on the situation (maybe you will have already existing configurations) you need to manually copy and paste this stuff. Copy all the files to the right destination with these commands:

```
cp -r ~/.dotfiles/.dreitagebart ~
cp -r ~/.dotfiles/.config ~
cp ~/.dotfiles ~/.tmux.conf
```

## Command line tools

- [Homebrew](https://brew.sh) - The Missing Package Manager for macOS (or Linux)

  ```
  /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
  ```

- [zsh](https://www.zsh.org) - A unix shell that can be used as an interactive login shell and as a command interpreter for shell scripting

  ```
  brew install zsh
  ```

- [oh-my-zsh](https://ohmyz.sh) - Delightful, open source, community-driven framework for managing your zsh configuration

  ```
  sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
  ```

- [fzf](https://github.com/junegunn/fzf) - Command line fuzzy finder

  ```
  brew install fzf
  ```

- [thefuck](https://github.com/nvbn/thefuck) - Magnificent app which corrects your previous console command.

  ```
  brew install thefuck
  ```

- [bat](https://github.com/sharkdp/bat) - A cat(1) clone with wings

  ```
  brew install bat
  ```

- [fd](https://github.com/sharkdp/fd) - A simple, fast and user-friendly alternative to 'find'

  ```
  brew install fd
  ```

- [eza](https://github.com/eza-community/eza) - Modern, maintained replacement for ls

  ```
  brew install eza
  ```

- [zoxide](https://github.com/ajeetdsouza/zoxide) - A smarter cd command. Supports all major shells

  ```
  brew install zoxide
  ```

- [neovim](https://neovim.io) - Hyperextensible Vim-based text editor

  ```
  brew install neovim
  ```

- [ripgrep](https://github.com/BurntSushi/ripgrep) - Recursively searches directories for a regex pattern while respecting your gitignore

  ```
  brew install ripgrep
  ```

- [nerdfont](https://www.nerdfonts.com) - Patches developer targeted fonts with a high number of glyphs (icons)

  ```
  mkdir -p ~/.local/share/fonts
  cd ~/.local/share/fonts && curl -fLO https://github.com/ryanoasis/nerd-fonts/raw/HEAD/patched-fonts/DroidSansMono/DroidSansMNerdFont-Regular.otf
  ```

  ! After that set this font in your terminal - perhaps you must restart your shell

- [tmux](https://github.com/tmux/tmux) - A terminal multiplexer \
  In many distros tmux is preinstalled - see [installation instructions](https://github.com/tmux/tmux/wiki/Installing)

- [tpm](https://github.com/tmux-plugins/tpm) - tmux plugin manager installs and loads tmux plugins
  ```
  git clone https://github.com/tmux-plugins/tpm ~/.tmux/plugins/tpm
  ```
  ```
  tmux && tmux source ~/.tmux.conf
  ```
  Type `Control + Space` and `I` (a capital I for installing the tmux plugins)

## Development tools

- [nvm](https://github.com/nvm-sh/nvm) - Node version manager - a POSIX-compliant bash script to manage multiple active node.js versions

  ```
  curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.7/install.sh | bash
  ```

- [pnpm](https://pnpm.io) - Fast, disk space efficient package manager

  ```
  npm install -g pnpm
  ```

- [yarn](https://classic.yarnpkg.com) - Fast, reliable and secure dependency management
  ```
  npm install -g yarn
  ```

## Post installation steps

After installation of all that stuff add following lines at the end of your `~/.zshrc` file:

```
source $HOME/.dreitagebart/.aliasrc
source $HOME/.dreitagebart/.configrc
source $HOME/.dreitagebart/.evalrc
```
