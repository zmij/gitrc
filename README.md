Initially found this script somewhere in the internet. Patched to work with different colors for clean branch, dirty branch, stages changes.

Installation:

Place the file .gitrc to your home directory. Add the following code to your .bashrc file:

if [ -f ~/.gitrc ]; then
        . ~/.gitrc
fi

Sometimes the terminal doesn't set the variable color_prompt correctly, so if you want to get a colored prompt, just add force_color_prompt=yes before if [ -n "$force_color_prompt" ] line.

