# CVR-Problem
Solving the Capacitated Vehicle Routing Problem with different heuristics


## Table of contents
* [General info](#general-info)
* [Setup](#setup)

## General info
Team lab project for Algorithms and Data Structures III.

There are a series of n points numbered from 1 to n, 1 being the central deposit and the rest representing clients  

## Setup
To run this project, choose a possible heuristic {savings, goloso, sweep, 2-opt, annealing}, samples are to be chosen from the data file.  

```
$ make clean && make
$ cat data/sample.vrp | ./build/vrp --algo HEURISTIC
```

For help:

```
$ ./build/vrp --help

```

