---
layout: page
title: "User Guide"
permalink: /user-guide/
---

## Contents
{:.no_toc}

- TOC
{:toc}

## Getting Started

### Downloading and Running ISSIE

Start by clicking the [download](https://github.com/tomcl/issie/releases/latest) button on the top-right of your screen. This opens the page of the latest release of ISSIE on GitHub. At the bottom of the page, you can find the latest prebuilt binary for your platform (Windows or Macos). Issie will require in total about 200M of disk space.

- **Windows:** unzip \*.zip anywhere and double-click the top-level `Issie.exe` application in the unzipped files.
- **Macos:** Double click the dmg file  and run the application inside the folder, or drag and drop this to install.
    - The binaries are not signed. You will need to [perform a one-off security bypass](https://www.wikihow.com/Install-Software-from-Unsigned-Developers-on-a-Mac).
    

### Creating a New Project

Once you open Issie you should see two options: `New Project` and `Open Project`. 
  
- Click `New Project`
- Navigate to the folder you want to save your project
- Enter the name of your project
- Click `Create Project`

This process creates a folder where your project will be stored and the first sheet of your project, called `main`. You can see this by clicking at the `Sheets` selection button.

### Your first design

Let's start with a very simple schematic: a simple 2-input AND gate. 

Add the following components to your canvas from the `Catalogue` tab:
- `INPUT/OUTPUT` => `Input` => Name: 'A', Bits: 1
- `INPUT/OUTPUT` => `Input` => Name: 'B', Bits: 1
- `GATES` => `And` 
- `INPUT/OUTPUT` => `Output` => Name: 'OUT', Bits: 1

Now make the appropriate wiring to connect all the components by clicking on one port and dragging the wire to the port you want to connect it to. 
**Connect:**
- Input 'A' to the first input port of the AND gate
- Input 'B' to the second input port of the AND gate
- Output 'OUT' to the output port of the AND gate

Your design should look like this:

![](../img/userGuide/firstDesign.gif)


### Simulation

Time to simulate our design and see how the output `OUT` changes as we change the two inputs BLAH.

Click the `Simulation` tab which is located on the top-right corner and then `Start Simulation`. Now you can change the value of the two inputs and see how the value of the output. Try all 4 combinations of inputs: 
- A=0, B=0  
- A=0, B=1  
- A=1, B=0  
- A=1, B=1 
   
and check that the output is correct based on the truth table of the AND gate.

![](../img/userGuide/firstDesignSim.gif)


**Well Done!** You just completed your first ISSIE design.  

## Exploiting the ISSIE Features

### A slightly more complex design

Time to increase the complexity of our design and see how we can exploit the features of ISSIE to create clean and good-looking schematics.

- Add two more inputs named `C` and `D` each 1-bit.
- Add one OR gate and one 2-input MUX
- Delete the output `OUT`
  - Note: You can delete components and/or wires by selecting them and clicking the `delete` button on your keyboard
- Add a new 1-bit output `RESULT`   
- Make all necessary connections to achieve a diagram like the one bellow:

![](../img/userGuide/features1.png)

Again, **simulate the design** and check the output remains correct as you change the values of the 4 inputs

### Improving the looking of our design

Clearly, this is a terrible and hard to understand design. **Let's improve it!** The ISSIE canvas is fully customisable to allow the creation of readable and good-looking schematics. Specifically, we can:
1. Rotate, Flip and Move around all symbols 
2. Change and Move around the symbols' labels
3. Manually route wires as you like
4. Auto-align elements 
5. Select the wire type we desire (radiussed, jump or modern wires)

You can view the shortcuts for all these modifications by clicking on the `edit` and `view` menus.

**Let's now look at our improved schematic:**

![](../img/userGuide/features2.gif)


### Summary

- In the `Catalogue` Menu we can find an extensive and complete library of components (gates, flip-flops, RAMs, ROMs, n-bit registers)
- We can add any number of components in our sheet and name them as we like
- When clicking on a port, ISSIE shows us all the ports we can connect that port to. 
- Wires are initially automatically routed
- We can modify our schematic as we like to create a good-looking design.
- We can simulate our design and check how the outputs change as we change the inputs.


## Using Custom Components