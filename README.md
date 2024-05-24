# Installation instructions

## Command line tools

- [Homebrew](https://brew.sh) - The Missing Package Manager for macOS (or Linux)

  ```
  /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
  ```

- [zsh](https://www.zsh.org) - A unix shell that can be used as an interactive login shell and as a command interpreter for shell scripting

  ```
  brew install zsh
  ```

- [oh-my-zsh](https://ohmyz.sh) - Delightful, open source, community-driven framework for managing your Zsh configuration

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
