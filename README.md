# PG Starter Config

I made this parental guidance starter config for my nephews who're younger than 13.

## Install

1. Download this repo
1. Unzip it
1. If your folder structure is `pg-config-master/pg-config-master` save the inner folder and delete the outer folder
1. Move the remaining folder into your `tf/custom` folder
1. Navigate into the `cfg` folder: `tf/custom/pg-config-master/cfg` to add your configurations
1. Feel free to rename `pg-config-master`

## Chat Control

### Text Chat

Defaults to `chatOff` and `chatUnbind`

Console commands:

- `chatOff`: Turns text chat view off
- `chatOn`: Turns text chat view on
- `chatUnbind`: Unbinds `y` and `u` text chat interactions
- `chatBind`: Binds `y` and `u` text chat interactions

### Voice Chat

Defaults to `voiceOff`

Console commands:

- `voiceOff`: Turns voice chat off
- `voiceOn`: Turns voice chat on

_Note: There's a TF2 bug with controlling the voice chat through the console. To turn the voice on, **after** entering `voiceOn` in the console, you'll need to go into Options>Voice and check the box "Enable voice in this game", then press Apply._

## Game Settings

### General

- FOV 90
- Min-viewmodels on
- Autoreload on
- Hitsounds on
- Combat text on; batching on
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
