# openFPGA-Gyruss

Gyruss-compatible openFPGA core for Analogue Pocket. Ported directly from the 
original [MiSTer core](https://github.com/MiSTer-devel/Arcade-Gyruss_MiSTer)
by [Ace](https://github.com/Ace9921) and [MiSTer-X (MrX-8B)](https://github.com/MrX-8B). 

## Controls

Controls are mapped as follows on the Analogue Pocket:

| Function | Keys |
|--|--|
| Ship Movement |  D-Pad |
| Fire: face buttons |
| Insert Coin: | Select (-) |
| Start | Start (+) |

Additional button mapping is supported via the "input" menu.

## Interact Menu

The core provides an "interact" menu, allowing a user to adjust DIP switches and other
hardware controls.

DIP Switches:

- Starting lives (3, 4, 5, or 255)
- Bonus live scores (30k/90k/60k+ or 40k/110k/70k+)
- Difficulty level (8 settings)
- Cabinet Type (Upright or Cocktail)
- Enable or Disable Demo Sounds + Demo Music

Game reset and service mode can also be controlled from the interact menu from the Analogue Pocket OSD.

Note: Gameplay is paused while in the OSD.

## Known Limitations

* High Score saving unimplemented.
* Pause is unimplemented.

## License

Source code for the openFPGA integration of this core is provided under the
terms of GPLv3. Please see the component repositories for licensing details
of individual modules. 

## Attribution

All credits for the Gyruss-compatible FPGA core are due the original authors
and contributors, for which this port would not have been possible. Credits
for the original work (taken from the original 
[core documentation](https://github.com/MiSTer-devel/Arcade-Gyruss_MiSTer?tab=readme-ov-file#credits))
are as follows:

```
Sorgelig - MiSTer project lead
MiSTer-X - Original Gyruss core design (https://github.com/MrX-8B/MiSTer-Arcade-Gyruss)
Ace - New Gyruss core design & Konami custom chip implementations
ElectronAsh - Assistance with Konami custom chip implementations
Artemio Urbina - Hardware references for video and audio output
JimmyStones - High score saving support & pause feature
Kitrinx - ROM loader
ThePulseRifle - Playtesting
```

```
---------------------------------------------------------------------------------
-- T80/T80s - Z80 compatible microprocessor core  Version 0242
-- Copyright (c) 2001-2002 Daniel Wallner (jesus@opencores.org)
---------------------------------------------------------------------------------
-- SYNTHEZIABLE CPU09 - 6809 compatible CPU Core  Version 1.4 (Modified)
-- Author: John E. Kent (dilbert57@opencores.org)
---------------------------------------------------------------------------------
-- T8039 Microcontroller System
-- Copyright (c) 2004, Arnim Laeuger (arniml@opencores.org)
---------------------------------------------------------------------------------
-- YM2149 (AY-3-8910)
-- Copyright (c) MikeJ - Jan 2005
---------------------------------------------------------------------------------
```

## Installation

Copy the contents of the "dist" folder to the root of the SD card, along with the converted ROM file as described below.

### ROM Instructions

ROM files are *not included*, you must use [mra-tools-c](https://github.com/sebdel/mra-tools-c/)
along with the provided `Gyruss.mra` to convert a MAME-compatible romset to a singular
`gyruss.rom` file compatible with this core.  This ROM file should be placed under
`/Assets/gyruss/obsidian.Gyruss`.
