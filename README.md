We use locate to search your home directory. It is normally much quicker than
find. It is designed to work with Python 3.6

We do not run locate if no parameters are supplied because it slows down
startup of Rofi a lot. We also make startup as quick as possible by only
doing imports and defining functions when we need to do some work.

If this file is named rofi-fb then it will launch gnome-terminal, if it is
named rofi-gfb it will launch nemo. You should change it to whatever you
like 😉 Make a hard link from rofi-fb to rofi-gfb.

Run this python script as a shell script, i.e.: rofi -show window -modi
"drun,run,fb:<path to dir containing rofi-fb>/rofi-fb"  
