---
layout: default
title: Rowan
permalink: /module/rowan/
---

## Rowan

<a href="../../images/rowan/rowan-front.jpg" target="_blank"><img title="" src="../../images/rowan/rowan-front-thumb.jpg" alt="" height="128" width="128"></a><a href="../../images/rowan/rowan-side.jpg" target="_blank"><img src="../../images/rowan/rowan-side-thumb.jpg" height="128" width="128" /></a><a href="../../images/rowan/rowan-rear.jpg" target="_blank"><img src="../../images/rowan/rowan-rear-thumb.jpg" height="128" width="128" /></a><a href="../../images/rowan/rowan-pcbs.jpg" target="_blank"><img src="../../images/rowan/rowan-pcbs-thumb.jpg" height="128" width="128" /></a>

Rowan is the second expander to [Sycamore](../sycamore) adding some additional outputs and a scale display.

To complement Sycamore's quantized to a scale outputs, Rowan adds unquantized and chromatic outputs which allow for passing the random sequence to other quantizers, or for use as CV sources. Similar to [Oak](../oak), Rowan also includes a pair of trigger outputs which fire as the Chromatic note changes for the left and right hand sides.

To allow for the easier visualisation of Sycamore's scales, Rowan has a colourful LED display which shows the currently active notes and give feedback as to what exactly changing the Scale and Quantize controls are doing to the allowed notes.

(Youtube demo video to follow)

<!-- {% include youtube.html id="Z_jfuflqjoc" %} -->

## Technical Information

- 12hp, 1U
- Trigger outputs active for 50ms at 5v
- Quantized and Unquantized outputs 0-5v.
- 40mA peak on +12v, -12v and 5v rails unused. Reverse-polarity protection on the power input. More LEDs lit may draw a little more power
- Chainable i2c headers reserved for future use, or for you own hacking

## Patch examples

Rowan is a relatively small and simple module but there are some neat patches that you might consider trying out....

### Complementary lines

Modules required:

- Sycamore
- Rowan
- VCOs or another sound source
- Supporting modules for the VCOs, if required (VCAs, VCFs, envelopes)
- A clock source
- A quantizer with control over specific notes to be played. For example, the Sonic Potions Penrose or Intellijel Scales

Patch one of Oak's unquantized outputs to the second quantizer module. Pick a few notes that you wish to complement the main melody. If the quantizer has a trigger input, patch Rowan's trigger output to it. Now, as Sycamore is clocked, Rowan will produce the raw, unquantized stream of random for the second quantizer to make use of. 

This technique works best if the second quantizer is set to a scale similar to Sycamore's currently active scale, but play around with different sets of active notes to uncover unexpected complementary combinations.

## Resources

- [BOM](https://github.com/tpcarlson/synth-diy/blob/main/rowan/BOM.md)
- [Assembly Guide](https://github.com/tpcarlson/synth-diy/blob/main/rowan/ASSEMBLY.md)
- [Firmware Guide](https://github.com/tpcarlson/synth-diy/blob/main/rowan/FIRMWARE.md)
- [Manual](https://github.com/tpcarlson/synth-diy/blob/main/rowan/MANUAL.md) (Manual to follow)

## Availability

Rowan will be available soon on Tindie and Reverb.

<!-- Sycamore is available as a [kit from Tindie](https://www.tindie.com/products/divergentwaves/sycamore/), or as a built module on [Reverb](https://reverb.com/uk/item/80138906-divergent-waves-sycamore). -->

## Special thanks

This module would not exist without the sketch from Mutable Instrument's [Cancelled Projects](https://pichenettes.github.io/mutable-instruments-documentation/trivia_and_history/cancelled_projects/) page on which Sycamore's design was based.

A special shoutout also to the Red Means Recording, Modular in a Week and Winterbloom Discord communities.