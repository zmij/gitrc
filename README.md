Initially found this script somewhere in the internet. Patched to work with different colors for clean branch, dirty branch, staged changes. For a clean branch the color is different if there are pending local or remote changes.

It looks like this:

![gitrc](https://cloud.githubusercontent.com/assets/2694027/3011768/0abf2b16-df30-11e3-817d-b804097345b1.png)

## Installation

Place the **.gitrc** file to your home directory. Add the following code to your **.bashrc** or **.profile** file:

```shell
# uncomment this line if your startup script doesn't set color_prompt correctly
# color_prompt=yes
if [ -f ~/.gitrc ]; then
        . ~/.gitrc
fi
```

## Automatically updating remote

The remote changes can be automatically updated. This can be a time consuming operation, so a reasonable update interval shoud be chosen. The feature is disabled by default and it can be set by

```Shell
# Set remote update interval in seconds
git config --local prompt.updateinterval 60
```

To turn automatic remote update off

```shell
git config --local --unset prompt.updateinterval
```
