remesher
========

A simple feature-preserving isotropic remesher based on edge flips, edge collapses and vertex repositioning.

This is pre-alpha code forked and adpated from https://github.com/jamesgregson/remesher

## Requirements

Working version of CMake is used to build this code

## Building

Generate makefiles using CMake from the build/ subdirectory then build with make.

```
<path>/remesher$ cd build
<path>/remesher/build$ cmake .. 
<path>/remesher/build$ make
```
## Meshing

After a successful build, run from bin/ subdirectory or play with the run_suite.py

Run with no options to see command line arguments, e.g.:

```
<path>/remesher/bin$ ./remesher
option -size defaulted to 0.02
option -feat defaulted to 45.0087
option -iters defaulted to 10
==================================================
Usage: ./remesher [parameters]
==================================================
Parameters:
  -input  <String>  [REQUIRED] input file in .obj format
  -output <String>  [REQUIRED] output file in .obj format
Optional parameters:
  -size   <Real>    [OPTIONAL] edge length as fraction of bounding box longest side, default: 0.02
  -feat   <Real>    [OPTIONAL] feature threshold, degrees, default: 45.0087
  -iters  <Integer> [OPTIONAL] number of remeshing iterations to perform, default: 10
==================================================
Errors: 
required option -input was not specified!
required option -output was not specified!

command line was: 
./remesher 
```

## Example outputs

![bunny](https://github.com/jamesgregson/remesher/blob/master/images/bunny.png)

![cad model](https://github.com/jamesgregson/remesher/blob/master/images/cad1.png)

![cad model](https://github.com/jamesgregson/remesher/blob/master/images/cad2.png)

![cad model](https://github.com/jamesgregson/remesher/blob/master/images/cad3.png)
