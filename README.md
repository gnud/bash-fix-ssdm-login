# bash scripts
(Ubuntu tested >=18.04)

Compatible with [Basher](https://github.com/basherpm/basher)

# Details

Imagine some day you open your laptop lid and you find your login screen all black with cursor on the middle, however your have so many apps opened and unsaved data, and your cannot afford crashing the X server.

Don't worry this script is on the rescue.

When can this happen, there is a bug on the nvidia drivers and screen don't get repainted and thus black screen.

One of the complaints:
https://forums.developer.nvidia.com/t/screen-randomly-flickers-flashes-to-black-on-kubuntu-18-04-with-nvidia-rtx-2080ti-and-driver-435-21/82500/2

One solution is to restart kwin with:
```bash
export KWIN_TRIPLE_BUFFER=1
kwin --replace
```

Unfortunetly it's harder to restart kwin, we need KDE session and stuff.

# Usage

Open a new tty in the virtual consoles, using control + alt + F(2..8) (tty1 is occupied by hte X server)
