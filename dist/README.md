# openFPGA-Gyruss

Gyruss-compatible openFPGA core for Analogue Pocket. Ported directly from the 
original [MiSTer core](https://github.com/MiSTer-devel/Arcade-Gyruss_MiSTer)
by [Ace](https://github.com/Ace9921) and [MiSTer-X (MrX-8B)](https://github.com/MrX-8B). 

## Features

* All DIP Switches

## Usage


## Known Limitations

* High Score saving unimplemented.
* Pause is unimplemented.

## License

Source code for the openFPGA integration is provided under the terms of GPLv3. 
Please see the component repositories for licensing details for the individual
components. 

## Attribution

Credits for the [original core](https://github.com/MiSTer-devel/Arcade-Gyruss_MiSTer?tab=readme-ov-file#credits)

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

## Special thanks

Special thanks to Ace for 

## ROM Instructions

ROM files are not included, you must use [mra-tools-c](https://github.com/sebdel/mra-tools-c/)
along with the provided `Gyruss.mra` to convert a compatible romset to a singular
`gyruss.rom` file.  Place the ROM file in `/Assets/gyruss/obsidian.Gyruss`.
