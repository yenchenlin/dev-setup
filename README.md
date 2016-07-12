# dev-setup
My VSLab development environment setup

## General
- `sudo apt-get install ssh`
- `sudo apt-get install vim`
- `sudo apt-get install git`

## zsh

- `sudo apt-get install zsh`
- `chsh -s /bin/zsh`
- `git clone git://github.com/robbyrussell/oh-my-zsh.git ~/.oh-my-zsh`
- `cp ~/.oh-my-zsh/templates/zshrc.zsh-template ~/.zshrc`

## tmux

- `sudo apt-get install tmux`
- Install [tmux-config](https://github.com/tony/tmux-config).


## Anaconda


## Cuda
- Download `.run` installer of Cuda 7.5 from [official site](https://developer.nvidia.com/cuda-toolkit).
- `sh` the download file.
- Edit `.bashrc` (`.zshrc` if you use zsh) to include the following lines:

  ```
  export PATH=/usr/local/cuda-7.5/bin:$PATH
  export LD_LIBRARY_PATH=/usr/local/cuda-7.5/lib64:$LD_LIBRARY_PATH
  ```

## Fisa Dev
- Install [fisadev](http://fisadev.github.io/fisa-vim-config/).

## Torch

## Tensorflow
