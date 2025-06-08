---
layout: default
title: Oneshot
permalink: /module/oneshot/
---

## Oneshot

<a href="../../images/oneshot/oneshot-front.jpg" target="_blank"><img title="" src="../../images/oneshot/oneshot-front-thumb.jpg" alt="" height="128" width="128"></a><a href="../../images/oneshot/oneshot-side.jpg" target="_blank"><img src="../../images/oneshot/oneshot-side-thumb.jpg" height="128" width="128" /></a><a href="../../images/oneshot/oneshot-rear.jpg" target="_blank"><img src="../../images/oneshot/oneshot-rear-thumb.jpg" height="128" width="128" /></a><a href="../../images/oneshot/oneshot-pcbs.jpg" target="_blank"><img src="../../images/oneshot/oneshot-pcbs-thumb.jpg" height="128" width="128" /></a>

Oneshot is an envelope generator with a number of interesting waveforms. Oneshot includes a big arcade button for manually triggering along with a trigger input.

Various parameters that control the Oneshot waves can be modulated including the duration of each wave, the number of repeats, time between repeats, and the waveform.

Oneshot also includes a small CV mixer section allowing for Oneshot's output to be mixed with another CV source.

Oneshot lends itself well to self-patching and experimentation as the CV and knob controls will change the wave on the fly, as parameters change.

{% include youtube.html id="v3djYLEpFeE" %}

## Technical Information

- 8hp
- Trigger inputs on over 1.1v, off under 1.1v
- CV inputs +/- 5v
- Output waveforms 0v to about 6.5v
- 40mA peak on +12v, 20mA -12v, with the 5v rail unused. Reverse-polarity protection on the power input

## Patch examples

Oneshot lends itself well to experimentation - feed the CV inputs some slow modulation and see what happens, or self-patch for a more chaotic output. Here are a couple of sample patches.

### Basic patch

Modules required:

- A sequencer, VCO, VCF, and VCA
- Oneshot

Patch together the sequencer, VCO, VCF, and VCA as a regular subtractive synth voice. Patch the sequencer's gate or clock output into Oneshot's Trigger input. 

Patch Oneshot's outputs to the VCA and VCF and you've got a little synth voice with an unconventional envelope! 

To expand on this patch, try changing the waveform, speed, and repeats to see how this affects the sound.

### Self-patching chaos

Modules required:

- A sequencer, VCO, VCF, and VCA
- Oneshot

Set up Oneshot in the same way as the basic patch above. Patch the Mix output back into the Duration input of Oneshot. Start the sequencer and see what happens! Now try the other CV inputs for more fun times.

Try patching the feedback through a VCA and modulating the amount of feedback with another LFO, or attenuating the feedback for more subtle changes and effects.

## Resources

- [BOM](https://github.com/tpcarlson/synth-diy/blob/main/oneshot/BOM.md)
- [Assembly Guide](https://github.com/tpcarlson/synth-diy/blob/main/oneshot/ASSEMBLY.md)
- [Manual](https://github.com/tpcarlson/synth-diy/blob/main/oneshot/MANUAL.md)

## Availability

Oneshot is available as a [kit from Tindie](https://www.tindie.com/products/divergentwaves/oneshot/), or as a built module on [Reverb](https://reverb.com/uk/item/90437258-divergent-waves-oneshot).

## Special thanks

With thanks to ElectricDruid for their wonderfully versatile little PIC chips, to arcadepartsuk for supplying buttons, and to the lovely people at SWS.