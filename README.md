# Windows Manager

i3wm

# Tools

Install all:

```
apt install libgconf-2-4 jq bc qalc git sshfs compton xautolock rxvt-unicode tmux rvm j4-dmenu-desktop fonts-font-awesome xbacklight i3blocks curl zsh
```

* i3blocks - for i3 bottom bar status
* compton - for animation effects when switching windows or workplaces
* xautolock - for locking screen
* rxvt-unicode - known as urxvt, base terminal
* tmux
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
* xbacklight - for controlling screen brightness

# Other

* bc
* curl
* jg - for parsing json from command line
* zsh - shell

# Sublime text

Installed packages:
* JSX
* CJSX Syntax
* Case Conversion
* Better CoffeeScript
* RailsCasts Colour Scheme
* Theme - Soda

# Oh my zsh configuration

Add following to ~/.zshrc
```
BUNDLED_COMMANDS=(rake rails rspec rubocop sidekiq cap guard)
plugins=(git bundler)
```
