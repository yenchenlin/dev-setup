# dev-setup
My development environment setup

# Linux

## General
- `sudo apt-get install ssh`
- `sudo apt-get install vim`
- `sudo apt-get install git`
- `sudo apt-get install g++` (**required** to install CUDA)

## zsh

- Install zsh, follow the reference [here](https://github.com/robbyrussell/oh-my-zsh/wiki/Installing-ZSH)
- `sh -c "$(wget -O- https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"`

## tmux

- `sudo apt-get install tmux`
- Install [tmux-config](https://github.com/tony/tmux-config).

## Anaconda
- Install miniconda 3.

## Cuda
- Download `.run` installer of Cuda 7.5 from [official site](https://developer.nvidia.com/cuda-toolkit).
- Open Ubuntu's `System Settings` and find `Software & Updates`
- Find section `Additional Drivers` and select `XXX (proprietary, tested)`
- `sh` the download file.

  **Note**: select **no** when system prompt ask you to install

  To verify if you've installed CUDA successfully, run following command
  ```
  cd /usr/local/cuda/samples/1_Utilities/deviceQuery
  sudo make
  ```
- Edit `.bashrc` (`.zshrc` if you use zsh) to include the following lines:

  ```
  export PATH=/usr/local/cuda-7.5/bin:$PATH
  export LD_LIBRARY_PATH=/usr/local/cuda-7.5/lib64:$LD_LIBRARY_PATH
  ```

## Vim
- Copy [this](https://github.com/amix/vimrc/blob/master/vimrcs/basic.vim) into `~/.vimrc`.

## Visual Studio

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
