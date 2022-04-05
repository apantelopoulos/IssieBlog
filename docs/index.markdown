---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: default
title: "Home Page" 
---

# Contents
{:.no_toc}

- TOC
{:toc}

# What is Issie

**I**nteractive **S**chematic **S**imulator and **I**ntegrated **E**ditor **(ISSIE)** is a very easy to use and capable hierarchical block schematic based digital logic editor and simulator, originally made for the 1st year undergraduate Digital Electronics and Computer Architecture module at the Department of Electronic and Electrical Engineering, Imperial College London, by 3rd year students at the same institution.

Issie has been well tested on designs with up to 15,000 schematic components. We expect it to be reasonably performant on much larger designs as well. The simulation speed is approximately 2000 component-clocks per ms. Thus a circuit with 1000 components would run at 2000 clocks per second. Issie creates fully synchronous circuits with a single clock: logic with asynchronous loops is currently not supported.

Issie is coded in F# transpiled to Javascript by [FABLE](https://www.fable.com), and uses a pure F# drawing library.

# Key Features

## Component Library

ISSIE has an extensive and complete library of components available in the 'Catalogue' menu. Components include low-level gates and flipflops as well as larger blocks: RAMs, ROMs, n-bit registers and adders. The lack of HDL-based combinational logic is partly filled by special components: Bus Select (extracts a bit-field), Bus Compare (decodes a min-term of a bus). Components defined as Verilog combinational logic are a likely future addition.


Viewer components are used to (optionally) view simulation waveforms of nodes on subsheets. Wire label components allow any number of nodes on one design sheet to be connected without visible wires.

<img src="img/catalog.png" alt="Catalog" width="800" height="400" center/>


## Wire Routing

## Width Inference

## Circuit Simulation

### Step Simulation
{:.no_toc}

### Waveform simulation
{:.no_toc}

## Verilog Output

## Memory Editor

# User Guide

# Developer Info

# Acknowledgements

# Contact