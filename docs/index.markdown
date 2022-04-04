---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home
---

# Issie

## What is Issie

Issie (Interactive Schematic Simulator and Integrated Editor) is a very easy to use and capable hierarchical block schematic based digital logic editor and simulator, originally made for the 1st year undergraduate Digital Electronics and Computer Architecture module at the Department of Electronic and Electrical Engineering, Imperial College London, by 3rd year students at the same institution.

Issie has been well tested on designs with up to 15,000 schematic components. We expect it to be reasonably performant on much larger designs as well. The simulation speed is approximately 2000 component-clocks per ms. Thus a circuit with 1000 components would run at 2000 clocks per second. Issie creates fully synchronous circuits with a single clock: logic with asynchronous loops is currently not supported.

Issie is coded in F# transpiled to Javascript by [FABLE](https://www.fable.com), and uses a pure F# drawing library.
