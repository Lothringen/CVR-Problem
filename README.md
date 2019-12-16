# CVR-Problem
Solving the Capacitated Vehicle Routing Problem with different heuristics


## Table of contents
* [General info](#general-info)
* [Setup](#setup)

## General info
Team lab project for Algorithms and Data Structures III.

As part of the graph theory seen in this subject, to solve this problem we can represent geographical points as nodes, and roads that connect them as edges. 
There are a series of n points numbered from 1 to n, 1 being the central deposit, and the rest of the points representing the clients to be visited. Each connected pair of points has an associated cost, which is the cost of moving between them. On the other hand, each point also has a demand that should be satisfied.
The deposit has an unlimited amount of vehicles, all with the same capacity C.
The problem consists in finding a group of minimum cost routes, that meet the following:
* Each point is visited exactly once, except for the deposit, by only one of the vehicles.
* Each vehicle begins and ends its route in the deposit.
* The sum of the demands of the clients visited by one vehicle cannot exceed its capacity C. 

## Setup
To run this project, choose a possible heuristic {savings, goloso, sweep, 2-opt, annealing}, samples are to be selected from the data file.  

```
$ make clean && make
$ cat data/sample.vrp | ./build/vrp --algo HEURISTIC
```

For help:

```
$ ./build/vrp --help

```

