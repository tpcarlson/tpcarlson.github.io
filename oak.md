---
layout: default
title: Oak
permalink: /module/oak/
---

## Oak

<a href="../../images/oak/oak-front2.jpg" target="_blank"><img title="" src="../../images/oak/oak-front2-thumb.jpg" alt="" height="128" width="128"></a><a href="../../images/oak/oak-side.jpg" target="_blank"><img src="../../images/oak/oak-side-thumb.jpg" height="128" width="128" /></a><a href="../../images/oak/oak-rear.jpg" target="_blank"><img src="../../images/oak/oak-rear-thumb.jpg" height="128" width="128" /></a><a href="../../images/oak/oak-pcbs.jpg" target="_blank"><img src="../../images/oak/oak-pcbs-thumb.jpg" height="128" width="128" /></a>

Oak is an expander to [Sycamore](../sycamore) which adds some useful features to the original module. Trigger outputs on every step, every note change, and at the start of each loop allow for creative patches that stay in time with the melody. Scale shuffle, previously only accessible via a long press on Sycamore, expands Sycamore with interesting patch-programmable quantization options.

The loop can be reset back to the first step after a trigger input or button press.

Sycamore's four main parameters that control the loop - Shift, Quantize, Length, and Range - may also be locked at the press of a button.

{% include youtube.html id="Zvx0Bf0yH-E" %}

<!-- {% include youtube.html id="Z_jfuflqjoc" %} -->

## Technical Information

- 7hp
- Trigger inputs on over 1.1v, off under 1.1v
- Trigger outputs active for 50ms at 5v
- 50mA peak on +12v, -12v and 5v rails unused. Reverse-polarity protection on the power input
- Chainable i2c headers reserved for future use, or for you own hacking

## Patch examples

Oak adds a lot of flexibility to Sycamore, but it is best thought of in three parts: Parameter locking, trigger outputs, and scale manipulation.

### Triggered scale shuffling

Modules required:

- Sycamore
- Oak
- VCOs or another sound source
- Supporting modules for the VCOs, if required (VCAs, VCFs, envelopes)
- A clock source

Patch Sycamore's outputs to the VCO 1v/oct inputs, and the clock source into Sycamore's clock input. Patch Oak's Start of loop output into its scale shuffle input. Pick a scale, set the quantize control to about 1/4 and the Length control to about the same, then set the clock running. 

Now, every time the loop repeats, Oak will trigger a scale shuffle. While the structure - notes rising or falling - will remain the same, Sycamore will pick a new subset of the notes to be shuffled as part of the scale. This works really well with Quantize set to less than about half, and adds some melodic variation to an otherwise static pattern.

### Step and Note-based triggers demo

Modules required:

- Sycamore
- Oak
- A VCO
- Supporting modules for the VCO, if required (VCA, VCF, envelopes)
- A switched multiple such as the Doepfer [A-182](https://doepfer.de/a182.htm)
- A clock source

Patch Sycamore to a VCO and all the usual VCO supporting modules. Patch Oak's Note and Step outputs to a switched multiple, and the switched multiple to the envelope generator. Patch the clock source to Sycamore's clock input and set the sequence running.

With the switched multiple, toggle between Oak's Note and Step outputs to drive the envelope generator. With Step, every clock of Sycamore will be replicated with a small delay as Sycamore changes the pitch. Repeated notes will trigger the envelope. Change this to Note and most clock inputs to Sycamore will trigger the envelope generator, but when there are two repeated notes the envelope generator will not be triggered. This is very useful for making more rhythmically interesting patches!

## Resources

- [BOM](https://github.com/tpcarlson/synth-diy/blob/main/oak/BOM.md)
- [Assembly Guide](https://github.com/tpcarlson/synth-diy/blob/main/oak/ASSEMBLY.md)
- [Firmware Guide](https://github.com/tpcarlson/synth-diy/blob/main/oak/FIRMWARE.md)
- [Manual](https://github.com/tpcarlson/synth-diy/blob/main/oak/MANUAL.md)

## Availability

Oak is available as a [kit from Tindie](https://www.tindie.com/products/divergentwaves/oak/), or as a built module on [Reverb](https://reverb.com/uk/item/85429774-divergent-waves-oak).

<!-- Sycamore is available as a [kit from Tindie](https://www.tindie.com/products/divergentwaves/sycamore/), or as a built module on [Reverb](https://reverb.com/uk/item/80138906-divergent-waves-sycamore). -->

## Special thanks

This module would not exist without the sketch from Mutable Instrument's [Cancelled Projects](https://pichenettes.github.io/mutable-instruments-documentation/trivia_and_history/cancelled_projects/) page on which Sycamore's design was based.

A special shoutout also to the Red Means Recording, Modular in a Week and Winterbloom Discord communities.