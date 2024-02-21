# MDP REPRESENTATION

## AIM:

To represent any one real-world problem in MDP form

## PROBLEM STATEMENT:

### Problem Description

Develop a game application where an agent promotes players upon level clearance and demotes upon loss using reinforcement learning.

### State Space
```
{A1,A2,A3}--> {0,1,2}
A1--> LEVEL 1
A2--> LEVEL 2 
A3--> LEVEL 3

```
### Sample State

A1--> 0 --> LEVEL 1

### Action Space
```
{W,L}-->{0,1}
W-->True
L-->False
```

### Sample Action

W--> 0 --> True

### Reward Function

R = { +1 , if we come closer to the winning
       0 , if not

### Graphical Representation

![image](https://github.com/lisianathiruselvan/mdp-representation/assets/119389971/f681c1d9-ac89-4c20-829e-1418d4f0b4e3)


## PYTHON REPRESENTATION:
```
P = {
    0:{
        0: [(0,1,1,True)],
        1: [(1.0,0,1.0,False)]
    },
    1:{
        0: [(0,2,1,True)],
        1: [(1,0,1,False)]
    },
    2:{
        0: [(0,2,1,True)],
        1: [(1,1,1,False)]
    }
}
P

```
## OUTPUT:

![image](https://github.com/lisianathiruselvan/mdp-representation/assets/119389971/bc3e32ca-4302-4702-ac47-6b74fe191c2c)


## RESULT:

Thus the given real world problem is successfully represented in a MDP form .
