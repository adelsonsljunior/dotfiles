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
stow -t ~/ [folder-to-deploy]
~~~

## Tilix

> For `tilix` don't use stow, use **dconf** instead.

~~~bash
#save
dconf dump /com/gexperts/Tilix/ > tilix/tilix.dconf
~~~


~~~bash
#load
dconf load /com/gexperts/Tilix/ < tilix/tilix.dconf
~~~