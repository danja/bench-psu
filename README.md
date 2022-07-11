# bench-psu

*A power supply for electronics experimentation*

## Status

*2022-07-11* - returning to this after a long pause. 

* I've got two 32v laptop PSUs
* I made and populated a front panel
* I've got some LM317s to use as the main components
* I bought a couple of very cheap V/A displays, DSN-VC288, nearest thing to a datasheet is [here]()

I need to figure out the circuit...


See [devlog.md](devlog.md)

## Specifications

Provisionally :

 * Dual variable max. 30v, with variable current limit max. 500mA.
 * Fixed 0 - 3.3 - 5 - 9v

## Motivation

I play with transistor/op amp circuits as well as Arduino & similar microcontrollers. For a long time I've been making do with a fixed +/- 12v supply I knocked together for the analog, little 3.3/5v PSU modules for the digital. A work-in-progress (https://github.com/danja/analog-computer) needs +/- 15v, so time to make something a bit more versatile. 

## Components



![some bits](https://github.com/danja/bench-psu/blob/master/images/bits_2020-09-25.jpeg?raw=true "Some bits")

With PSU in mind I bought a couple of cheapo digital display V/A meters (Banggood, China), everything else things I have knocking around.

I've got a bunch of LM317 regulators so the main circuits will be based on these.

I've got two very similar old HP switch mode PSUs (from printers?), each with +16v & +32v around 700mA. Transformers are expensive, so I might as well recycle these. The plan is to use the 32v from each to source the variable outputs. Not sure yet, but probably use one to also source the fixed outputs. 
(The minimum voltage out for each channel, is likely to be at least 1.5v thanks to the LM317s, maximum will likely be a bit less than 30v, but it's very rare I want beyond those edges).

For a case, I had a 3mm sheet aluminium offcut that cut in half & cleaned up provides pieces 146x148mm that I plan to use for the front and back panels. I've also got quite a large 14mm thick plywood board which should do for the sides. Low cost beats aesthetics there.

I've got some stripboard I can build the circuit on.

I've 4mm connection posts for the variable supplies, 2mm sockets for the fixed voltages.

### Front Panel

It hardly seems worth bothering about this for something so simple, a one-off. But I have other projects in progress where a nice front panel will be important, so playing with approaches here should be useful.

In the recent past I made a reasonable-looking front panel using laminate designed for signs, hand-drilled, with the symbols printed on a sheet of transparent acetate. For the design I used LibreOffice Draw. This worked ok, straightforward, but not ideal if I wanted to use a service to machine-cut panels. So this time trying Inkscape for the design.

Getting there :

![front panel](https://github.com/danja/bench-psu/blob/master/images/front-panel.png "front panel")






