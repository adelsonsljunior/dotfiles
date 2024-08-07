# dotfiles

## Prepare Workstation

Install Stow
~~~bash
sudo apt install stow -y
~~~

Clone this repository

~~~bash
git clone https://github.com/adelsonsljunior/dotfiles.git && cd dotfiles
~~~

## Apply the configuration

~~~bash
stow tmux
~~~

## Tilix

> For `tilix` don't use stow, use **dconf** instead.

~~~bash
dconf load /com/gexperts/Tilix/ < tillix/tilix.dconf
~~~