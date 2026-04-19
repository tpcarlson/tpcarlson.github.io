---
layout: default
title: Cyclic
permalink: /module/cyclic/
---

## Cyclic

<a href="../../images/cyclic/front.jpg" target="_blank"><img src="../../images/cyclic/front-thumb.jpg" height="128" width="128" /></a><a href="../../images/cyclic/top.jpg" target="_blank"><img src="../../images/cyclic/top-thumb.jpg" height="128" width="128" /></a><a href="../../images/cyclic/rear.jpg" target="_blank"><img src="../../images/cyclic/rear-thumb.jpg" height="128" width="128" /></a><a href="../../images/cyclic/pcbs.jpg" target="_blank"><img src="../../images/cyclic/pcbs-thumb.jpg" height="128" width="128" /></a>

Cyclic is an 8 channel, 16 step sequencer. Cyclic's channels can each be clocked individually, and each channel also has a separate trigger output. Cyclic also outputs MIDI notes and can be used as a controller for drum machines and anything else that talks MIDI.

With each channel clocked individually, Cyclic is perfect for exploring polyrhthms. Cyclic is deliberately very simple - there is no copy and paste, saving of sequences, pattern chaining, song mode, generation of sequences, support for polymeters or euclidean sequences. Instead, the focus is squarely on what you can do with polyrhthmic patterns.

If you're not feeling polyrhythmic, Cyclic copies input clocks from the first channel to the second and so on when clock inputs are unpatched. This allows for clocking it with a single clock input, or (For example) splitting Cyclic into two halves clocked at different rates.

Cyclic's user interface is the 128-button grid, with 16 steps per sequence. The button pads are backlit with LEDs to show when a step is active, triggered, or inactive.

While many sequencers want to be the main clock in your system, or want a very regular and unchanging clock, Cyclic gets out of the way and will happily accept whatever clocks it is passed. Each clock pulse increments the sequence once, so if you have a Eurorack system and want to use a module that outputs swung clocks or irregular clocks, Cyclic will deal with them just fine. If you're feeling adventurous you could also try other sources of voltage like an LFO or even a low-frequency VCO.

## Technical Information

- 8 clock inputs
- 8 trigger outputs
- MIDI out for each sequencer channel
- MIDI in exists, but is unused in the current firmware
- 250mm x 140mm x 40mm
- Customisable trigger length and MIDI note generation
- USB-C for editing configuration
- 5v barrel socket for regular use (A 5v supply with at least 2A output is recommended)
- 3D printed, two-part case

## Patch examples

Cyclic should be plug-and-play for the most part, but here are some example patches.

### Drive another sequencer

Modules & equipment required:

- Cyclic
- A second eurorack sequencer, patched to a sound source (VCO)
- A eurorack clock source
- An envelope generator, VCA, VCF, and VCO

Patch the clock source into the first of Cyclic's clock inputs. Patch the trigger input below the clock input on the rear panel to the clock input of the sequencer. Now you can start the clock and activate steps on Cyclic's button pads to increment the clock on the second sequencer. This is most helpful if you want to clock a sequencer at an irregular rate.

Try activating a second set of Cyclic's pads after patching the second trigger output to an envelope. Triggering of the envelope and the advancing of the sequencer clock at different times, at different amounts during a 16 step cycle, can lead to some interesting evolving patterns...

### Drum triggers

Modules & equipment required:

- Cyclic
- A clock source
- A drum machine

Patch Cyclic's MIDI output to a drum machine using an appropriate cable. Cyclic uses TRS-MIDI type A, but you can also use a TRS-A to MIDI DIN converter.

Patch a clock source into Cyclic's first trigger input.

Now start the clock, activate steps on Cyclic and you've got a very simple drum trigger sequencer.

Try patching a second clock source and see how that affects how you sequence the drums. The second clock might be a division or multiplication of the first, or a clock with a completely different tempo.

## Resources

Manual and assembly guide to follow.

<!--

- [Manual](https://github.com/tpcarlson/synth-diy/blob/main/cyclic/MANUAL.md)
- [Assembly guide](https://github.com/tpcarlson/synth-diy/blob/main/cyclic/ASSEMBLY.md)
-->

## Availability

Cyclic is currently a working prototype. I do have a few spare PCBs left from the second round of protyping, and I'm happy to 3D print a case too. If you are interested in purchasing a PCB set, case, or a full Cyclic device, please email me (hello@divergentwaves.co.uk).

<!--

Dice is available as a [kit from Tindie](https://www.tindie.com/products/divergentwaves/dice/), or as a built module on [Reverb](https://reverb.com/uk/item/79834786-divergent-waves-dice). Takazudo Modular also stocks built Dice modules on [Mercari](https://jp.mercari.com/shops/product/D7FxJkfnUAq24f4xVBUE2M).
-->