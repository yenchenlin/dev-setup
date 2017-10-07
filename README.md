# dev-setup
My VSLab development environment setup

## General
- `sudo apt-get install ssh`
- `sudo apt-get install vim`
- `sudo apt-get install git`
- `sudo apt-get install g++` (**required** to install CUDA)

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

## ~/.vimrc
- copy [this](https://github.com/amix/vimrc/blob/master/vimrcs/basic.vim) into `~/.vimrc`.

## Torch

## Tensorflow
