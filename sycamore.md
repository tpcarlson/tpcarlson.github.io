---
layout: default
title: Sycamore
permalink: /module/sycamore/
---

## Sycamore

<a href="../../images/sycamore/sycamore-front.jpg" target="_blank"><img src="../../images/sycamore/sycamore-front-thumb.jpg" height="128" width="128" /></a><a href="../../images/sycamore/sycamore-side.jpg" target="_blank"><img src="../../images/sycamore/sycamore-side-thumb.jpg" height="128" width="128" /></a><a href="../../images/sycamore/sycamore-rear.jpg" target="_blank"><img src="../../images/sycamore/sycamore-rear-thumb.jpg" height="128" width="128" /></a><a href="../../images/sycamore/sycamore-pcbs.jpg" target="_blank"><img src="../../images/sycamore/sycamore-pcbs-thumb.jpg" height="128" width="128" /></a>

Sycamore is a random looping sequencer with quantization and a wide range of scales. The quantized loop can be shifted, mutated, tweaked and otherwise fiddled with in a number of interesting ways.

With CV over almost all the internal parameters, Sycamore allows for tight control over the loop, while maintaining performability with comfortably spaced knobs.

Some advanced features are accessible through a one-layer menu to allow for more deep tweaking of harmonies, delay, and scale quantization - however, Sycamore is perfectly usable without touching these at all!

Sycamore makes use of CircuitPython for its program code, allowing for easy modification and tweaking should you wish to do so. The module also features an i2c expansion port reserved for future use, or for you own hacking.

{% include youtube.html id="Z_jfuflqjoc" %}

## Technical Information

- High-quality 12-bit DAC (LTC2632)
- 12HP
- 60mA peak on +12v, 10mA peak on -12v (5v rail unused). Reverse-polarity protection
- Trigger & Clock inputs on over 1.1v, off under 1.1v
- CV inputs -5 to +5v
- Aux CV input 0 to +5v
- Negative input voltage protection on all signal inputs

## Patch examples

Sycamore is most at home as a dual quantized output. Here are a couple of simple examples.

### Basic use

Modules required:

- Sycamore
- A clock source
- A pair of VCOs
- Supporting modules for the VCOs, if required (VCAs, VCFs, envelopes)

Wire the clock source to Sycamore's clock input. Wire Sycamore's outputs to the two VCOs. Make sure the output mode is set to the first mode.

Now you can tweak the length, offset (With Shift), quantization, and range with the four controls in the center, and change the scale with the encoder.

Patch an LFO to one of the four CV inputs to automate knob-twiddling. Changing the quantization and range have the most immediate effects!

### Keyboard tracking with a VCF

Modules required:

- Sycamore
- A clock source
- A VCO
- An envelope generator
- A VCA
- A VCF with a 1v/oct input

Wire the clock source to both the envelope generator and Sycamore's clock input, Sycamore's output 1 to the VCO, and Sycamore's output 2 to the VCF. Set the envelope generator up to control opening and closing the VCA, and optionally add an attenuated copy of this to the VCF.

Hold the mode button to dive into mode tweaking and use the encoder to set the note offset to "00". This will make Sycamore output the same note to outputs 1 and 2. Now clock Sycamore, and you should hear the VCF's cutoff following the VCO pitch.

## Resources

- [BOM](https://github.com/tpcarlson/synth-diy/blob/main/sycamore/BOM.md)
- [Assembly Guide](https://github.com/tpcarlson/synth-diy/blob/main/sycamore/ASSEMBLY.md)
- [Firmware Guide](https://github.com/tpcarlson/synth-diy/blob/main/sycamore/FIRMWARE.md)
- [Manual](https://github.com/tpcarlson/synth-diy/blob/main/sycamore/MANUAL.md)

## Availability

Sycamore is coming soon! If you would like one built for you, please <a href="../../">contact me</a>.

## Special thanks

This module would not be possible without the sketch from Mutable Instrument's [Cancelled Projects](https://pichenettes.github.io/mutable-instruments-documentation/trivia_and_history/cancelled_projects/) page. Sycamore expands on the ideas from Seeds, keeping the layout largely the same with some ergonomic and practical tweaks to make it a little easier to build and use and adding some additional functionality where it made sense to do so.

A special shoutout also to the Red Means Recording, Modular in a Week and Winterbloom Discord communities.