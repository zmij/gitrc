Initially found this script somewhere in the internet. Patched to work with different colors for clean branch, dirty branch, staged changes.

It looks like this:

![gitrc](https://cloud.githubusercontent.com/assets/2694027/3011768/0abf2b16-df30-11e3-817d-b804097345b1.png)

Installation:

Place the **.gitrc** file to your home directory. Add the following code to your **.bashrc** file:

```Shell
if [ -f ~/.gitrc ]; then
        . ~/.gitrc
fi
```

Sometimes the terminal doesn't set the variable **color_prompt** correctly, so if you want to get a colored prompt, just add **force_color_prompt=yes** before **if [ -n "$force_color_prompt" ]** line.

