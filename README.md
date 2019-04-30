# Windows Manager

i3wm

# Tools

Install all:

```
apt install libgconf-2-4 jq bc qalc git sshfs compton xautolock rxvt-unicode tmux mc j4-dmenu-desktop fonts-font-awesome i3blocks curl zsh scrot htop vim libpq-dev nodejs xclip httpie
```

* i3blocks - for i3 bottom bar status
* compton - for animation effects when switching windows or workplaces
* xautolock - for locking screen
* rxvt-unicode - known as urxvt, base terminal
* tmux
* polybar - bar for i3wm 
* httpie - https://httpie.org command line replacement for curl
* j4-dmenu-desktop - quick application launcher, faster then i3 built-in app
* rambox - google hangouts client
* fonts-font-awesome - fonts & icons for status bar
* ranger - command line file manager
* arandr - tool for managing monitors
* wicd-curses - command line network manager
* qalc - calculator
* network-manager-gnome - applet for managint internet connections
* zathura - for pdf preview
* feh - for image preview
* pcmanfm - file manager
* light - https://github.com/haikarainen/light for controlling screen brightness
* xclip - for clipboard to make it work with Visual Studio Code extensions

# Polybar installation

sudo apt-get install cmake cmake-data libcairo2-dev libxcb1-dev libxcb-ewmh-dev libxcb-icccm4-dev libxcb-image0-dev libxcb-randr0-dev libxcb-util0-dev libxcb-xkb-dev pkg-config python-xcbgen xcb-proto libxcb-xrm-dev i3-wm libasound2-dev libmpdclient-dev libiw-dev libcurl4-openssl-dev libpulse-dev libxcb-composite0-dev xcb libxcb-ewmh2

git clone https://github.com/jaagr/polybar.git

cd polybar && ./build.sh

# Other

* bc
* curl
* jg - for parsing json from command line
* zsh - shell

# Light configure

Install from deb package https://github.com/haikarainen/light/releases

Next allow to run through sudo without password

```
sudo visudo

```

And insert

```
Cmnd_Alias PASSWORDLESS = /usr/bin/light

# and at the bottom

%sudo   ALL=(ALL:ALL) NOPASSWD: PASSWORDLESS
```

# Oh my zsh configuration

Add following to ~/.zshrc
```
BUNDLED_COMMANDS=(rake rails rspec rubocop sidekiq cap guard)
plugins=(git bundler)
```

# Other

Configure tap to click on touchpad: https://ubuntuforums.org/showthread.php?t=2375454
