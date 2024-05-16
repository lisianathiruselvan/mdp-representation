# MDP REPRESENTATION

## AIM:

To represent a Markov Decision Process(MDP) problem in the following ways.

1.Text representation

2.Graphical representation

3.Python - Dictonary representation

## PROBLEM STATEMENT:

### Problem Description

The agent has to solve a problem statemnt using programming languages available and level up from easy to difficult to achive the goal state of earning a badge.

The agent can either level up or Level down the difficulty.

The probability of the agent being able to or unable to solve the problem given is 60%.

### State Space

0 - Easy Level

1 - Medium Level

2 - Hard Level

3 - Badge Earned (Goal State)

### Sample State

The agent is in the Medium Level Problem Statement (state=1)

### Action Space

0 - Level Down

1 - Level Up

### Sample Action

At State=1 (medium) the agent performs 0 (Level Down) and either

60% Levels Down to State=0 (easy)

40% Levels Up to State=2 (hard)

### Reward Function

R = {+1 if state = 3  
      0 otherwise}

## GRAPHICAL REPRESENTATION

![2](https://github.com/lisianathiruselvan/mdp-representation/assets/119389971/88741868-3afb-4248-8ffa-4d755d9c5813)

</BR>

## PYTHON REPRESENTATION:

### Developed by: Lisiana T
### Register Number: 212222240053

```

solver_mdp = {
    0: {
        1: [(0.6, 1, 0, False), (0.4, 0, 0, False)],
        0: [(0.6, 0, 0, False), (0.4, 1, 0, False)]
    },
    1: {
         1: [(0.6, 2, 0, False), (0.4, 0, 0, False)],
        0: [(0.6, 0, 0, False), (0.4, 2, 0, False)]
    },
    2: {
         1: [(0.6, 3, 1, True), (0.4, 1, 0, False)],
        0: [(0.6, 1, 0, False), (0.4, 3, 1, True)]
    },
    3: {
         1: [(0.6, 3, 0, True), (0.4, 3, 0, True)],
        0: [(0.6, 3, 0, True), (0.4, 3, 0, True)]
    }
}
```

## OUTPUT:
![1](https://github.com/lisianathiruselvan/mdp-representation/assets/119389971/4cb40049-bc7d-4739-8770-ab6d0bbc1d80)


## RESULT:

Thus the given Markov Decision Process(MDP) problem is represented in the following ways.
