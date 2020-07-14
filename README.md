# Kali terminal

This is my current terminal interface for Kali Linux.

tmux
-----
The tmux config is based on gpakosz "Oh my tmux". Go to https://github.com/gpakosz/.tmux for instructions or execute the following commands:

```
cd
git clone https://github.com/gpakosz/.tmux.git
ln -s -f .tmux/.tmux.conf
cp .tmux/.tmux.conf.local .
```
(Feeling confident? Don't make a backup of your .tmux config file ;))

Want to use my .tmux.conf.local to make the pink go away? 

```
git clone https://github.com/dspieard/kaliterminal.git
cp kaliterminal/.tmux.conf.local .
```

terminal theme
--------------
In terminal, go to file>preferences>Appearance and change the color scheme to "GreenOnBlack

powerline
---------
To get the nice looking arrows install powerline:

```
apt-get install powerline
```

Then edit the ~/.bashrc -file:

```
#Powerline
if [ -f `which powerline-daemon` ]; then
  powerline-daemon -q
  POWERLINE_BASH_CONTINUATION=1
  POWERLINE_BASH_SELECT=1
  . /usr/share/powerline/integrations/powerline.sh
fi
```
