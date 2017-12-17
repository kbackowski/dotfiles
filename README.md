# dotfiles

# Install urxvt and its dependencies

apt-get install rxvt-unicode xsl xclip
mkdir /usr/lib/urxvt/perl/
create file /usr/lib/urxvt/perl/clipboard with content:

#script to copy/paste text in URXVT

#! perl

sub on_sel_grab {
    my $query = $_[0]->selection;
    open (my $pipe,'| /usr/bin/xclip -in -selection clipboard') or die;
    print $pipe $query;
    close $pipe;
}

sub paste {
    my ($self) = @_;
    my $content = `/usr/bin/xclip -loop 1 -out -selection clipboard` ;
    $self->tt_write ($content);
}

sub on_user_command {
    my ($self, $cmd) = @_;
    if ($cmd eq "clipboard:paste") {
        $self->paste;
    }
}

# Windows Manager

i3wm

# Tools

* i3blocks - for i3 bottom bar status
* compton - for animation effects when switching windows or workplaces
* xautolock - for locking screen
* rxvt-unicode - known as urxvt, base terminal
* rambox - google hangouts client
* ranger - command line file manager
* arandr - tool for managing monitors
* wicd-curses - command line network manager
* qalc - calculator
* network-manager-gnome - applet for managint internet connections
* zathura - for pdf preview
* feh - for image preview
* pcmanfm - file manager
