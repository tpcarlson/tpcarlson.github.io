---
layout: default
title: DrumFiend
permalink: /module/drumfiend/
---

## DrumFiend

<a href="../../images/drumfiend/drumfiend-front.jpg" target="_blank"><img src="../../images/drumfiend/drumfiend-front-thumb.jpg" height="128" width="128" /></a><a href="../../images/drumfiend/drumfiend-side.jpg" target="_blank"><img src="../../images/drumfiend/drumfiend-side-thumb.jpg" height="128" width="128" /></a><a href="../../images/drumfiend/drumfiend-rear.jpg" target="_blank"><img src="../../images/drumfiend/drumfiend-rear-thumb.jpg" height="128" width="128" /></a><a href="../../images/drumfiend/drumfiend-pcbs.jpg" target="_blank"><img src="../../images/drumfiend/drumfiend-pcbs-thumb.jpg" height="128" width="128" /></a>

DrumFiend is a trigger-to-MIDI processor. Send it triggers, and it'll send out MIDI notes to a connected drum machine.

With the default firmware, DrumFiend is set up with a drum map for the DrumBrute Impact with each trigger input corresponding to a drum. Inputs on the left and right hand side are the normal and "colour" versions of the various drums, with trigger input 19 reserved for the cowbell.

DrumFiend's inputs trigger at levels above 2.5v and may be run all the way up to low audio rates.

As DrumFiend runs CircuitPython, changing the drum map to output different MIDI notes is as easy as plugging it in to your computer. You can even completely change the module's function if you want to!

DrumFiend supports both MIDI-A and MIDI-B TRS-MIDI variants, switchable with jumpers on the back of the module.

{% include youtube.html id="JPxy6Dy0QuU" %}
{% include youtube.html id="wxmLj0OS0Og" %}

## Technical Information

- 19 Trigger Inputs
- 1 MIDI output (MIDI-TRS, Type A or B)
- 8HP
- 40mA peak on +12v, -12v and 5v rails unused
- Inputs on over 2.5v, off under 2.4v

## Patch examples

DrumFiend isn't just for drums... here's a few examples of what you can do with it.

### Drums Triggers

Modules & equipment required:

- DrumFiend
- A source of triggers
- A drum machine

Patch the various trigger sources into DrumFiend's trigger inputs and the DrumFiend's MIDI output into a drum machine. That's it - instant modular-to-drum machine triggering.

### Running Drums at audio rates

Modules required:

- A VCO, or fast LFO
- DrumFiend
- A drum machine

Similar to the first patch - run the LFO or VCO into one of the DrumFiend trigger inputs and DrumFiend's MIDI output into a drum machine. Try setting the VCO/LFO to around 1000Hz to start with and see what your drum machine does - you might get nothing, or you might get something strange.

For the DrumBrute Impact, experiment with the FM drum. Tune the mod and carrier pitch, the FM amount and the decay and use your drum machine as a weird VCO...

## Resources

- [Manual](https://github.com/tpcarlson/synth-diy/blob/main/drumfiend/MANUAL.md)
- [Firmware Info](https://github.com/tpcarlson/synth-diy/blob/main/drumfiend/FIRMWARE.md)
- [Assembly guide](https://github.com/tpcarlson/synth-diy/blob/main/drumfiend/ASSEMBLY.md)

## Availability

DrumFiend is available as a [kit from Tindie](https://www.tindie.com/products/divergentwaves/drumfiend/), or as a built module on [Reverb](https://reverb.com/uk/item/79834463-divergent-waves-drumfiend)