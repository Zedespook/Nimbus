# This is a public fork of Fuzion, since this is a public cheat, use it on your own risk!

[![Join the chat at https://gitter.im/Aimtux-Fuzion/Lobby](https://img.shields.io/gitter/room/TechnologyAdvice/Stardust.svg?style=flat-square)](https://gitter.im/Aimtux-Fuzion/Lobby#)

Want to chat or play with other Fuzion users? Join us on Gitter!

# Changelog
Version 1.0.2 (Jan 25)
- Adjusted auto-defuser
- Adjusted backtrack
- Removed anti-aim debug duplicate in menus
- Added key save for third-person

Version 1.0.1 (Jan 16)
- Added player move-state based anti-aim
- Thirdperson angle is now last-tick viewangle
- Automatic LBY breaker values (customs are still available)
- Added disable anti-aim on knife-held back
- Changed default third-person value from 30 to 150
- Removed angle-indicator

Version 1.0.0 (Jan 15)
- Added new anti-aim
- Anti-aim angle keys
- New pretty bullet tracer
- Removed air-stuck
- Removed jump-throw
- Added backtrack
- Fake-lag optimization (No fake-lag while standing still)


## What is Fuzion?

A fully featured internal hack for *CounterStrike : Global Offensive* written in C++.

## What is Zedeware?

It is a fork of Fuzion, keeping the style and mentality. The difference being is the added/optimized features.

## Compiling

**Note:** _Do NOT download or compile as the root user._

#### Download the dependencies required to build Fuzion/Zedeware:

If you are having problems compiling make sure you've got the latest version of `g++`.

[How to update g++](https://github.com/AimTuxOfficial/AimTux/wiki/Updating-your-compiler)

==================

__Ubuntu-Based / Debian:__
```bash
sudo apt-get install cmake g++ gdb git libsdl2-dev zlib1g-dev patchelf
```
__Arch:__
```bash
sudo pacman -S base-devel cmake gdb git sdl2 patchelf
```
__Fedora:__
```bash
sudo dnf install cmake gcc-c++ gdb git libstdc++-static mesa-libGL-devel SDL2-devel zlib-devel libX11-devel patchelf
```

===================

#### Download Zedeware:

```bash
git clone --recursive https://github.com/LWSS/Fuzion
```

```bash
cd Fuzion
```

===================

#### Compile with build script

You can build easily with the included build script.
```bash
./build
```

You can later update with 
```bash
./update
```


## Injecting using the load script

First of all, make sure CS:GO is open, it does not matter whether you are in game or not. However, it is not recommended to inject while CS:GO is loading into a map. 

Navigate to the directory where Fuzion was built if you have not ready.
```bash
cd Fuzion
```

Now, you can inject the hack with the `load` script
```bash
./load
```

You might be prompted to enter in your password, this is because the injection script requires root access.

The text printed out during injection is not important. 

If the injection was successful you will see a message at the bottom saying `Successfully injected!`, however, if the message says `Injection failed`, then you've most likely done something wrong.

Now, go back into CS:GO, if you are in the main menu of the game you should see a banner in the top left like so:

![this](http://i.imgur.com/Gb0SV1u.png)

*Note:* if you are getting crashes ( that are unrelated to game updates ) Try disabling shader precaching in your Steam Client -> Steam -> Settings -> Shader Pre-Caching. 

## Using the hack

Now that Fuzion has been injected into the game, press <kbd>Insert</kbd> on your keyboard to open the hack menu (<kbd>ALT</kbd>+<kbd>I</kbd> if you are using a laptop).

If you want to change skins, create and load configs or open the player list, you can find those buttons at the top of the screen.


## Unloading the hack

If you wish to unload the hack from the game, you can do so by entering the command:
```bash
./uload
```

## Configs
# Your Fuzion configs can still be used on this cheat as well.

Configs are stored in a hidden directory in your home folder. Specifically 
```
~/.config/Fuzion
```

Each `config.json` is stored in a seperately named folder (The name you see in-game, in the config window). 

To add a config, create a folder inside of the `~/.config/Fuzion` folder with a name of your choice, and paste the `config.json` inside of that folder.

To see hidden folders inside your home folder, press <kbd>CTRL</kbd>+<kbd>H</kbd> when using a file manager.

On your command line, you can also add the -a flag on `ls` e.g.
```bash
ls -la ~/
```


## Grenade Configs

```
~/.config/FuzionGH
```

Each `config.json` is stored in the folder named after them map name.

To add a config, copy the folder containing it to `~/.config/FuzionGH`


## Screenshots

![aimbot](http://i.imgur.com/NhSEO9W.png)
![menu](http://i.imgur.com/59TGPfw.png)
![esp](http://i.imgur.com/lnF42Ng.png)


## Credits

Special thanks to the Original AimTux project: [https://github.com/AimTuxOfficial/AimTux](https://github.com/AimTuxOfficial/AimTux).

Special thanks to [@aixxe](http://www.github.com/aixxe/) ([aixxe.net](http://www.aixxe.net)) for the skin changer and with the initial project, as well as helping this project with source code (Available on [@aixxe's](http://www.github.com/aixxe/) github page.).

This project was also originally based upon Atex's [Linux Basehook](http://unknowncheats.me/forum/counterstrike-global-offensive/181878-linux-basehook.html).

[telans](https://github.com/telans) for the AUR package [fuzion-git](https://aur.archlinux.org/packages/fuzion-git/)

The Zedeware project is also glad to know [@LWSS](http://www.github.com/LWSS/) who is still providing us with quality code.
Special thanks to [@acuifex](http://www.github.com/acuifex/) for helping with the project a lot.
