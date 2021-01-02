# bash scripts
(Ubuntu tested >=18.04)

Compatible with [Basher](https://github.com/basherpm/basher)

# Details

Imagine someday you open your laptop lid and you find your login screen all black with the cursor on the middle, however, you have so many apps opened and unsaved data, and you cannot afford to crash the X server.

Don't worry this script is on the rescue.

When can this happen, there is a bug on the Nvidia drivers and the screen don't get repainted and thus black screen.

## Bugs listed

- https://forums.developer.nvidia.com/t/screen-randomly-flickers-flashes-to-black-on-kubuntu-18-04-with-nvidia-rtx-2080ti-and-driver-435-21/82500/2


## Workarounds

One solution is to restart "kwin" using the following code:

```bash
export KWIN_TRIPLE_BUFFER=1
kwin --replace
```

Unfortunately, it's harder to restart "kwin", we need KDE session id and stuff.

# Usage

Open a new TTY in the virtual consoles, using control + alt + F(2..8) (tty1 is occupied by the X server)
