# dev-setup
My development environment setup

# Linux

## General
- `sudo apt-get install ssh`
- `sudo apt-get install vim`
- `sudo apt-get install git`
- `sudo apt-get install build-essential` (**required** to install CUDA)
- Settings -> Displays -> Night Light -> Set the time to be the same

## zsh

- `sudo apt install zsh`
- `sh -c "$(wget -O- https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"`
- Add the following to `.zshrc` to prevent git command autocompletion to be slow:
```
__git_files () { 
    _wanted files expl 'local files' _files     
}
```

## tmux

- `sudo apt-get install tmux`
- Install [tmux-config](https://github.com/tony/tmux-config).

## Anaconda
- Install miniconda 3.

## Cuda
- See [this](https://medium.com/@exesse/cuda-10-1-installation-on-ubuntu-18-04-lts-d04f89287130)

## Vim
- Copy [this](https://github.com/amix/vimrc/blob/master/vimrcs/basic.vim) into `~/.vimrc`.

## Visual Studio

# Windows

WSL2, Ubuntu 22.04.1

## NVIDIA

- Drivers
- CUDA Toolkit

## Tools

- VSCode
- HWInfo
- MSI Afterburner
- GPU-Z
- Windows Power Toys
    - Remap keys of magic keyboard.

## Terminal

1. Click on the drop down menu -> Settings -> Open JSON file (left bottom)
2. Add this line: `"wordDelimiters" : " ()\"':,;<>~!@#$%^&*|+=[]{}~?\u2502",` to select paths in the shell with double clicks. 

## COLMAP

- Follow COLMAP's [instruction](https://colmap.github.io/install.html#linux) but install Ceres solver using its [own instruction](http://ceres-solver.org/installation.html). 

# MacOS

## Oh-my-zsh
- Follow the instruction [here](https://ohmyz.sh/)

## Homebrew
- Follow the instruction [here](https://brew.sh/)

## wget
`brew install wget`

## tmux

- `brew install tmux`
- Install [tmux-config](https://github.com/tony/tmux-config).

## Visual Studio

## Anaconda
- Install miniconda 3.

## Vim
- Copy [this](https://github.com/amix/vimrc/blob/master/vimrcs/basic.vim) into `~/.vimrc`.

## Flux
- Download it [here](https://justgetflux.com/).
