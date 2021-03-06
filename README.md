# DotFiles

My dotfiles to share configuration between workspaces 

## Prerequisites

1. Install **git** `sudo apt install git`
1. Install **tmux** `sudo apt install tmux`
1. Install **tpm** `git clone https://github.com/tmux-plugins/tpm ~/.tmux/plugins/tpm`
1. Install **Vim** `sudo apt install vim`
1. Install **Vundle** `git clone https://github.com/VundleVim/Vundle.vim.git ~/.vim/bundle/Vundle.vim`
1. Install **urlview** `sudo apt install urlview`
1. Install **wmctrl** `sudo apt install wmctrl`
1. Install **taskwarrior** `sudo apt install taskwarrior`
1. Install **pip** `sudo apt install python3-pip`
1. Install **time tracking hook for taskwarrior** `pip3 install taskwarrior-time-tracking-hook`
  - Add hook to taskwarrior
  ```
  mkdir -p ~/.task/hooks
  ln -s `which taskwarrior_time_tracking_hook` ~/.task/hooks/on-modify.timetracking
  ```

Run `install.sh` to create symlinks to your home folder

## Contents

- [install.sh](install.sh) - installation script (creates symlinks to your home directory)
- [.aliases](.aliases) - Shared (between *bash* and *zsh*) command aliases
- [.vimrc](.vimrc) - [Vim](https://www.vim.org/) configuration
- [.bashrc](.bashrc) - [Bash](https://www.gnu.org/software/bash/) config
- [.zshrc](.zshrc) - [Zsh](http://www.zsh.org/) config
- [.tmux.conf](.tmux.conf) - TMUX configuration
- [.taskrc](.taskrc) - Taskwarrior configuration

### Useful scripts/commands

- [.scripts/zenmode.sh](.scripts/zenmode.sh) - toggle Zen mode (disable arrow keys, disable mouse, enable full screen) alias `zen` 
- [.scripts/webcammpv.sh](.scripts/webcammpv.sh) - Show window in the bottom-right corner with streamed video from webcam. (Usefull for screencasts if you whant to make your videos more personalized)
