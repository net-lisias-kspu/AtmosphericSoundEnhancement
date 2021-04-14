# Atmospheric Sound Enhancement /L Unofficial

A plugin for Kerbal Space Program which models the effect of atmosphere on sound heard.

Unofficial fork by Lisias.


## In a Hurry

* [Latest Release](https://github.com/net-lisias-kspu/AtmosphericSoundEnhancement/releases)
	+ [Binaries](https://github.com/net-lisias-kspu/AtmosphericSoundEnhancement/tree/Archive)
* [Source](https://github.com/net-lisias-kspu/AtmosphericSoundEnhancement)
* Documentation
	+ [Project's README](https://github.com/net-lisias-kspu/AtmosphericSoundEnhancement/blob/master/README.md)
	+ [Install Instructions](https://github.com/net-lisias-kspu/AtmosphericSoundEnhancement/blob/master/INSTALL.md)
	+ [Change Log](./CHANGE_LOG.md)
	+ [TODO](./TODO.md) list


## Description

Adds the effects of the density, temperature and relative speed of the atmosphere to craft sounds. When breaking the sound barrier, muffled sounds (or optionally no sounds) will be heard when the camera is outside of the shock cone. When passing through the cone, you can hear the shockwave. When leaving the atmosphere, the sound gradually fades to muffled (or optionally nothing) in vacuum. Internally, sounds can always be heard but are muffled.

The stock game's condensation effects are now visible when travelling at transonic velocities. The plasma re-entry effects are visible when travelling at hypersonic velocities, regardless of altitude.

### Settings

* `negativeSlopeWidthDeg`
	+ The angle (in degrees) behind the shock cone that the shock wave fades away over.
* `interiorVolumeScale`
	+ A multiplier for the volume inside the craft. 1 is 100%, 0.5 is 50%, 2 is 200%, 0 for silence.
* `interiorMaxFreq`
	+ How muffled the sounds heard inside the craft are. Sounds above this frequency aren't heard. It can be anywhere between 10 (a deep rumble that can only be h
eard with high-quality speakers) and 22000 Hz (not muffled at all). 0 disables internal sounds.
* `lowerMachThreshold`
	+ The Mach number at which the sonic boom starts to kick in.
* `upperMachThreshold`
	+ The Mach number at which the sonic boom finishes fading away.
* `maxDistortion`
	+ How distorted and crunchy the sound of the shock wave is. 0 is off (normal) and 1 is on fully (may cause crackling).
* `condensationEffectStrength`
	+ How thick the white graphical condensation effect is when passing through the sound barrier. 0 is off, 1 is very thick.
* `maxVacuumFreq`
	+ How muffled the sounds are when in a vacuum, similar to interiorMaxFreq. 0 disables all sounds, 22000 gives normal, unmuffled sounds.
* `maxSupersonicFreq`
	+ How muffled the sounds are when the camera is ahead of the supersonic shock wave., similar to interiorMaxFreq. 0 disables all sounds, 22000 gives normal, un
muffled sounds.

### Acknowledgments

Thanks to velusip and szdarkhack for their major contributions to this mod. The plugin also makes reference to Deadly Reentry for compatibility with its particle effects.


## Installation

Detailed installation instructions are now on its own file (see the [In a Hurry](#in-a-hurry) section) and on the distribution file.

## License:

This work is licensed under the [GPLv2](https://opensource.org/licenses/GPL-2.0). See [here](./LICENSE).

Please note the copyrights and trademarks in [NOTICE](./NOTICE).


## UPSTREAM

* [pizzaoverhead](https://forum.kerbalspaceprogram.com/index.php?/profile/26349-pizzaoverhead/) ROOT
	+ [Forum](https://forum.kerbalspaceprogram.com/index.php?/topic/51558-*/)
	+ [CurseForge](https://www.curseforge.com/kerbal/ksp-mods/atmospheric-sound-enhancement/files)
	+ [Github](https://github.com/pizzaoverhead/AtmosphericSoundEnhancement)
