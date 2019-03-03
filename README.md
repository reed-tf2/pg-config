# PG Starter Config

I made this parental guidance starter config for my nephews who're younger than 13.

## Install

1. Download this repo
1. Unzip it
1. If your folder structure is `pg-config-master/pg-config-master` save the inner folder and delete the outer folder
1. Move the remaining folder into your `tf/custom` folder
1. Feel free to rename `pg-config-master`
1. Navigate into the `cfg` folder: `tf/custom/pg-config-master/cfg`
1. Open `custom.cfg` to adjust the settings

## Game Settings

### PG Settings

- Default `chatOff` -- `chatOn`/`chatOff`
- Default `voiceOff` -- `voiceOn`/`voiceOff`
- Default `unbindChat` -- `bindChat`/`unbindChat`
- Default `goreOff` -- `goreOn`/`goreOff`
- Default `spraysOff` -- `spraysOn`/`spraysOff`

### General

- FOV 90
- Min-viewmodels on
- Autoreload on
- Hitsounds on
- Damage numbers on; batching on
- Unbind \` key; bind toggleconsole key to F11 (easy to accidentally hit the \` key)

### Medic

- Autoheal off (will teach better I think)
- Autocallers on; threshold 99

### Sniper

- Play sound when fully zoomed 1

### Soldier

#### Rocket Jump Script

Disabled by default. To enable, open `soldier.cfg` and uncomment this line (remove the slashes):

```
bind MOUSE2 +rocketJump
```

It's bound to right mouse click (MOUSE2). This is fine for the stock rocket launcher, but it disables the right-click for the Cow Mangler. You can change the key in that file, but you need to reset that key to its [default behavior](https://wiki.teamfortress.com/wiki/List_of_default_keys) inside `reset.cfg`.

### Spy

- Concise disguise menu on

## Bugs

### Voice control commands

There's a TF2 bug with controlling the voice chat through the console. To turn the voice on:

1. Enter `voiceOn` in the console
1. Open **Options>Voice** and check the box "Enable voice in this game", then press Apply. If it's already checked, uncheck it and press Apply, then re-check it and press Apply.
