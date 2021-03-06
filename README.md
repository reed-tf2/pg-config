# Parental Guidance Config

A parental guidance config for Team Fortress 2 (TF2).

This config disables some vulgar language and imagery (from gamers on the internet), and enables a few settings that I recommend to beginners. It doesn't change any default gameplay controls.

I made this for my nephews who're younger than 13. Gamers reliably use language and imagery that aims to irk. They can learn all about that once they're a bit older. [#okboomer](https://i.giphy.com/PnggNmuamz7kbgfUTL.gif)

For more information about configs, how to install them, and how they work, I recommend reading this [Reddit TF2 Script Help](https://www.reddit.com/r/tf2scripthelp/wiki/introduction#wiki_using_scripts) post.

## Install

Installing this requires you to download this PG Config folder and put it in a specific TF2 folder. Then, when TF2 starts it will load the config.

Follow the folder paths precisely:

1. [Download](https://github.com/rufio-tf2/pg-config/archive/master.zip) this config
1. Unzip it
1. Unzipping can create an extra folder on Windows. If your folder structure is `pg-config-master/pg-config-master`, save the inner folder and delete the outer folder.
1. Open your `tf` folder:
   1. In the Steam "Library", right-click Team Fortress 2, select Properties:<br/>
      <img alt="`Properties` option at the bottom of the list" src="./assets/tf2_local_files_1.png" height="40%" width="40%" />
   1. Click the Local Files tab:<br/>
      <img alt="`Local Files` tab" src="./assets/tf2_local_files_2.png" height="50%" width="50%" />
   1. Click Browse Local Files:<br/>
      <img alt="`Browse Local Files` button" src="./assets/tf2_local_files_3.png" height="50%" width="50%" />
1. Navigate into the `tf/custom` folder
1. Move the `pg-config-master` folder into the `tf/custom` folder
1. Double check the folder structure. Starting in the `tf` folder, these folders need to exist in this order: `tf/custom/pg-config-master/cfg/`

## Game Settings

These can be adjusted in: `tf/custom/pg-config-master/cfg/custom.cfg`.

For more info, see these instructions [How To Adjust Settings](./docs/ADJUST_SETTINGS.md).

### PG Settings

Default settings are **bold**.

- **`voiceOff`**/`voiceOn`
- **`chatOff`**/`chatOn`
- **`unbindChat`**/`bindChat`
- **`goreOff`**/`goreOn`
- **`spraysOff`**/`spraysOn`
- Remove Conscientious Objector models ([How to re-enable](./docs/ENABLE_CONSCIENTIOUS_OBJECTOR.md))

### General

- FOV 90
- Min-viewmodels on
- Autoreload on
- Hitsounds on
- Damage numbers on; batching on
- Bind crouch to <kbd>SHIFT</kbd> key (easier for smaller hands)
- Unbind <kbd>\`</kbd> key; bind `toggleconsole` to <kbd>F11</kbd> (easy to accidentally hit the backtick key)

### Medic

- Autoheal on
- Autocallers on; threshold 99

### Sniper

- Play sound when fully zoomed

### Soldier

#### Rocket Jump Script

Disabled by default. To enable, open `soldier.cfg` and uncomment this line (remove the slashes):

```
bind MOUSE2 +rocketJump
```

It's bound to right mouse click (MOUSE2). This is fine for the stock rocket launcher, but it disables the right-click for the Cow Mangler. You can change the key in that file, but you need to reset that key to its [default behavior](https://wiki.teamfortress.com/wiki/List_of_default_keys) inside `reset.cfg`.

## Known Issues

### Voice control commands

There's a TF2 bug with controlling the voice chat through the console. To turn the voice on:

1. Enter `voiceOn` in the console
1. Open **Options > Voice** and check the box "Enable voice in this game", then press Apply. If it's already checked, uncheck it and press Apply, then re-check it and press Apply.

## Any problems?

Please [open a new issue](https://github.com/rufio-tf2/pg-config/issues/new/choose) to let me know.

## Contributing

Contributions are welcome and encouraged.

## Thanks

From the [Reddit post](https://www.reddit.com/r/Tf2Scripts/comments/awj06v/parental_guidance_config/):

- @bythepowerofscience for reminding me about the gore
- @byParallax for reminding me about the Conscientious Objector
- @JarateKing for helping me remove the Conscientious Objector models
- @woofbarkbro for reminding me to turn off sprays
