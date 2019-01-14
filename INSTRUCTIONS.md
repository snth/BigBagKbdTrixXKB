# INSTRUCTIONS #

To install the necessary files in the /usr/share/X11/xkb directory (after
making a backup of the current settings), run the following:

    ./install-dreymar-xmod.sh

Then to try out the new layout settings in the current terminal, run the
following:

    ./setxkb.sh

To make the xzorak keyboard permanent, add the following to your ~/.bashrc:

    setxkbmap -option ''    # need to first disable old option before we can set new ones
    setxkbmap -layout xzorak -variant xzorak1 -option 'misc:extend,lv5:lwin_switch_lock,xzorak:shift_alt_ctrl'

