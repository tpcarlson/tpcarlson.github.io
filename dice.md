---
layout: default
title: Dice
permalink: /module/dice/
---

## Dice

<a href="../../images/dice/front.jpg" target="_blank"><img src="../../images/dice/front-thumb.jpg" height="128" width="128" /></a><a href="../../images/dice/side.jpg" target="_blank"><img src="../../images/dice/side-thumb.jpg" height="128" width="128" /></a><a href="../../images/dice/rear.jpg" target="_blank"><img src="../../images/dice/rear-thumb.jpg" height="128" width="128" /></a><a href="../../images/dice/pcbs.jpg" target="_blank"><img src="../../images/dice/pcbs-thumb.jpg" height="128" width="128" /></a>

Dice is a 6-output probabilistic signal router. The input may be routed to one or more of the six outputs, controlled by rolling the dice. A large, 7-segment LED display shows the most recently rolled number along with clock information.

Dice can be used to route audio or CV, and will route audio clicklessly provided the waveform crosses 0v.

Dice includes a few different modes which may be combined to influence the way in which the outputs can be activated, including:

- Exclusive mode – only one output may be active at a time
- Skip mode – activating an output prevents the output from being deactivated until reset
- Auto-reset mode – when in skip mode, reset once all outputs are in the skip state

Additionally, the dice can be rigged with the central fader, biasing the dice to roll certain numbers more often than others. Dice's outputs may also be toggled with the buttons at the bottom of the module.

{% include youtube.html id="M2XgcmQ6p9Y" %}

## Technical Information

- 1 input (CV or audio)
- Up to 6 outputs active at the same time
- Output normalled to 5v; Dice will produce gates with no input
- 16HP
- 50mA peak on +12v, 20mA peak on -12v. 5v rail unused
- Latching trigger inputs for clocks and controls

## Patch examples

Dice is designed around audio, but can be used for CV as well. Here are a couple of patch ideas to get you started.

### Effects and filter routing

Modules & equipment required:

- Dice
- A VCO
- Up to 6 VCO destinations. Filters, FX etc.
- A clock source

Patch the VCO to the In input, and the 6 outputs to as many output destinations as you want. Now patch a clock to the Roll input and your VCO will be routed to the outputs as the dice is rolled.

Try patching outputs 1-3 panned left and outputs 4-6 panned right to have your VCO bounce around the stereo field. Use the central fader to influence how often the VCO goes left or right.

### Drum triggers

As Dice outputs gates with nothing patched to the input, you can use it as a source for other modules' triggers.

Modules & equipment required:

- Dice
- DrumFiend, or another trigger to MIDI module
- A clock source
- A drum machine

Patch the clock source to Dice's Roll input, and Dice's 6 outputs to different inputs on the trigger to MIDI module. Clocking Dice will fire off new drum hits.

Try using the central fader to influence which drums are played, and play with the skip, exclusive, and auto-reset toggles to change how many outputs may be active at once.

## Resources

- [Manual](https://github.com/tpcarlson/synth-diy/blob/main/d6/MANUAL.md)
- [Assembly guide](https://github.com/tpcarlson/synth-diy/blob/main/d6/ASSEMBLY.md)

## Availability

Dice is available as a [kit from Thonk](https://www.thonk.co.uk/shop/divergent-waves-dice/). If you would like one built for you, please <a href="../../">contact me</a>.