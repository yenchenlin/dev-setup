# dev-setup
My development environment setup

## General
- `sudo apt-get install ssh`
- `sudo apt-get install vim`
- `sudo apt-get install git`
- `sudo apt-get install g++` (**required** to install CUDA)

## bash

- Install [bash-it](https://github.com/Bash-it/bash-it)

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

## vimrc
#### Style
- Copy [this](https://github.com/amix/vimrc/blob/master/vimrcs/basic.vim) into `~/.vimrc`.
#### Format
- https://github.com/Chiel92/vim-autoformat
- Add the following snippet into .vimrc:
```
let g:autoformat_verbosemode = 0
let g:formatters_python = ['yapf']
let g:formatdef_yapf = "'yapf -l '.a:firstline.'-'.a:lastline"
let g:autoformat_remove_trailing_spaces = 1
noremap <C-K> :Autoformat<CR>
```

## Tensorflow 
`pip install tensorflow-gpu`
