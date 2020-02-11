# m4c0-cpu

## Description

This is my second attempt at creating a CPU based on [Ben Eater][be]'s design.
My [first attempt][1st] had a stronger focus on replicating Ben's design as SMD,
then implement my own version. This approach was challenging due to the lack of
schematics back then. Now, Ben has the overall architecture in his website,
which allows a better planning ahead on how different parts talk to each other.

By the way, this is a [LibrePCB](https://librepcb.org) project!

## Objectives

These are the tenants of this project:

* **Fun to work with** - if something looks too hard, then find a funnier
  solution
* **Modular** - the final result will be like a giant robot from a
  [tokusatsu][toku]. Something like a microservice-like convoluted mess. Why?
  Because it's fun!

## Planned architecture

In a nutshell, each bus will be a PCB with card edge connectors for each of its
daughter boards. There are multiple cases, like the main bus, the ALU register
connections, etc.

Control signals will not be part of the bus, since there are more than 20 of
them, mostly used by a single target. Those signals will be connected with
dupont wires for simplicity.

## License

See [LICENSE.txt](LICENSE.txt).

[be]: https://eater.net/8bit
[1st]: https://github.com/m4c0/be-cpu
[toku]: https://en.wikipedia.org/wiki/Tokusatsu 

