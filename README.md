# Jedi Knight 2 configuration

This is my gaming configuration for the multiplayer mode of Jedi Knight 2


## What's inside

Optimal display for multiplayer. Brighten the game, use 2d images for objects, ..
Almost all keys are binded, some work like menus with choices: crash, anonymize,
print players connected to favorite servers (ASE), one key per saber style (DSAC),
admingun, record video, small hacks to prevent ban or to make a server lag,
a lite configuration for jkbot to see pseudo on top of people


## Make a backup of your config

Before you test this config, you should do a backup of your jk2 config. 

Within the game, run from the console the command `/writeconfig backup.cfg`


## Install

Put everything into your `<jk2 install path>/GameData/Base` folder. If the folder does not exist, create it.

The autoexec.cfg file is triggered when the game starts.
It will also name you Padawan and set Kyle Katarn with his blue saber, which is the default pseudo, model and saber color.
This is handy when you want to stay anonymous when you connect to a server.

If you need to execute the config during the game write in the console: `/exec zougi/start` or press the `b` key


## Usage

Connect to a server and test the keys :D

To display a list of available keys, write from the console the command:

```
/bindlist
```

If a key ask to validate a choice, push it again to get another choice. Usually the key next to it is the next or prev key.
To validate use `F1` unless you're asked to hit another key.

One of the first thing when I connect to a server is to configure my binding depending on my powers. I use the `j` key to set binding and powers.


## Particularities

It's a very complete configuration, if you open the files everything is commented, which is cool .. but it's commented in french
I used to play essentially from a laptop with azerty, there is high chances you will need to edit the config to match your game style.
the easiest way is to override the config from the game and save your config with command `writeconfig`,
then add an `exec your_config` at the end of the start script for example. But ideally I would advise to just edit manually the text files.


## Known issues

### Resolution

When I used to play the screen resolution was not as high as today.
In "affichage.cfg", replace r_mode line with these:

```
seta r_customheight "720"
seta r_customwidth "1280"
seta r_mode "-1"
```

### Download of map from the server directly

By default `cl_allowDownload` is disabled because there is (was?) an exploit using this feature so I prefer to enable it on demand.
