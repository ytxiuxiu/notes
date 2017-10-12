
# Introduction
```
3D printing
  layer-by-layer: 
    1. time-consuming; 
    2. support structure, waste material, difficult to remove
  -> motivate: freeform printing, wireframe printing, rotating platform printing.

Freeform: not layer-by-layer, freeform extrusion in the air, no support structure
Current issues:
  1. too much deviation
  2. require strong material

Rotating platform: eliminate support structure, reduce collision
Current issues:
  1. low DOF
  2. suddenly change layer direction, strength
  
  tubes, vases
  
Wireframes: low-fidelity preview, faster prototyping, more oppotunities to improve. Used by architects, sculptors and artists
Current issues:
  1. sagging
  2. low DOF
  

```
# Related Works


# Contribution

## Controlling System
An integrated system controlling both robotic arms and a 3d printing system

### System Architecture

#### Hardwares
* filament holder
* platform
* 3d printing control box
* extruder and holder
* fan holder - as small as possible
#### Softwares
* controller
  * simulation
    * opengl
  * command executor
  * driver
* urscript
  * command executor
  * status monitor
* 3d printing firmware
  * modified extruder controlling

## Freeform Printing
* slow movement - slow extrusion
* small step angle - slow extrusion
* high speed fan - faster solidified
* bigger nozzle - stable

### Freeform printing with solid core
* solid core: maintain the overall shape
* algorithm to generate the shape

### Slinky printing
**flat nozzle**???
**smaller angle step motor**???
3m7s / layer

## Rotating Platform Printing
### Generalised cylinder
* different modeling approach - carrier, profile - bezier path
* different layer-height within one layer - algorithm
* rotate between layers - strength
* no support structure needed

#### Tube Printing
* layer computing algorithm

#### Vase Printing
* path generating algorithm
* base-filling algorithm

## Wireframe Printing
Freeform + Rotating platform
* rotating platform -> never print vertically -> eliminate the sagging problem

Robotic control

# Evaluation
convert to mesh

compare
* possibility - to conventional
  * freeform
  * slinky
* time - to conventional
  * tube
  * cube
* quality - to conventional
* material usage - to conventional
  * tube
  * **how to measure**???
* strength - to RoboFDM

# Limitation


# Conclusion