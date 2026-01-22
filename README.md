# Frodo V4.2 Libretro

## Legal Notes 
Copyright &copy; Christian Bauer et al.

This is downstream fork of https://github.com/libretro/frodo-libretro/ aimed at Libretro implementation of a "Lite" COMMODORE 64 emulator (the Super Compatible variant is WIP). It has been based of original CVS repository via commit: [1529f8b](https://github.com/Apaczer/frodo4/commit/1529f8b86abb1e9c1de087fa06766105fa72d5e8)

## Build instructions
1. Clone this repo's libretro branch
```
git clone -b libretro --single-branch https://github.com/Apaczer/frodo4
```
2. Compile `frodo_libretro.so` core
```
make -j$(nproc) -f Makefile.libretro platfrom=<your_target>
```

## Controls

|RetroPad button|Normal-Action|
|---|---|
|R1|SHIFTED BUTTONS (ON-Hold)|

|RetroPad button|KEYBOARD_EMULATED-Action|
|X|ENTER c64-key|
|Y|SPACE c64-key|
|SELECT|RUN/STOP c64-key|
|START|Show virtual Keyboard (Toggle)|
|R1|SHIFTED BUTTONS (ON-Hold)|

|RetroPad button|KEYBOARD_EMULATED-Shifted-Action|
|---|---|
|A|F1 c64-key|
|B|F3 c64-key|
|X|C= c64-key|
|Y|F7 c64-key|
|D-Pad|Cursors c64-keys|
|START|F5 c64-key|

|RetroPad button|JOYSTICK_EMULATED-Action|
|A|Joystick fire 1|
|B|Joystick up|
|D-Pad|Joystick move control|

|RetroPad button|MOUSE_EMULATED-Action|
|A|Left mouse btn|
|B|Right mouse btn|
|D-Pad|Mouse move control|

In mouse emulation D-Pad and A/B buttons controls the mouse.

Two joysticks support. Switch automatically between port 1 & 2 with JOYPAD_SELECT btn, or in Control settings port used.