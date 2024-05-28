# Computer Code

> custom computer code that allows readers to reproduce the results.
***
## About

There are five code files and two data files: 
* Network_Visualization.ipynb, Symbolic_Calculation.ipynb, 2_Strategy_Simulation.ipynb, 3_Strategy_Simulation.ipynb, and 3_Strategy_Evolution.ipynb;
* Data_1.xlsx and Data_2.xlsx.

The Figure folder contains figures in the paper and more.

The notations in the code, expect for the figures, are consistent with those in the paper.


### Network_Visualization.ipynb
> Plot some common network structures.

* ##### Function
    * plotting

### Symbolic_Calculation.ipynb

* ##### Setting

    * 3 strategies in a networked population under the death-birth update rule

    * conventional Prisoner's Dilemma game

> 1. Compute and simplify expressions of payoff matrix, fixation probabilities and long-term abundances.
> 2. Compute payoff matrix for different extortion factors $\chi$.
> 3. Plot fixation probabilities and long-term abundances as functions of the extortion factor $\chi$.

* ##### Function
    * expressions: equations, solutions, ...
    * numerical computation
    * plotting


### 2_Strategy_Simulation.ipynb

* ##### Setting

    * 2 strategies in a networked population under the death-birth update rule

    * donation game

> 1. Perform simulations `without` mutation for different benefit-cost ratios $b/c$. Then display the results of fixation probabilities: a comparison between simulation results and theoretical results.
> 2. Perform simulations `with` mutation for a given benefit-cost ratio $b/c = 4$. Then display the results of long-term abundances: changes of population structure over time.

* ##### Function
    * simulation
    * plotting


### 3_Strategy_Simulation.ipynb

* ##### Setting
  
    * 3 strategies in a networked population under the death-birth update rule

    * conventional Prisoner's Dilemma game

> 1. Perform simulations for different extortion factors $\chi$.
> 2. Display the results:
>   * (i) changes of population structure over time for two specific extortion factors $\chi = 1$ and $\chi = 4$;
>   * (ii) a comparison between simulation results and theoretical results.

* ##### Function
    * simulation
    * plotting


### 3_Strategy_Evolution.ipynb

* ##### Setting
  
    * 3 strategies in a lattice population under the death-birth update rule
    
    * with mutation

> Plot screenshots of the evolution process.
> > one of the three strategies may occupy the entire population at special steps

* ##### Function
    * plotting


### Data_1.xlsx

> This date file records the simulation results of long-term abundances simulated by the corresponding function in 3_Strategy_Simulation.ipynb.

> `original` and `average` data

We would like to visualize long-term abundances of strategies given different extortion factors. 
* We run 8 identical and independent simulations of $10^7$ generations and calculate the average values.
* Then, we use the average values to plot simulation results and compare them with theoretical results.

> The payoff structures with different extortion factors are given in Symbolic_Calculation.ipynb.


### Data_2.xlsx
> This date file records the simulation results of fixation probabilities simulated by the corresponding function in 2_Strategy_Simulation.ipynb.

> `original` data

We would like to visualize fixation probabilities between strategies given different benefit-cost ratios $b/c$ on different network structures. 
* For each strategy in each setting, we run $10^6$ independent simulations and calculate the chance it taking up the population to estimate its fixation probability.
* Then, we use the estimated values to plot simulation results and compare them with theoretical results.

***
## Instructions

The code is organized into ipython notebooks. 

The software, module and hardware list is given below.

* Software

> Python 3.8.8 and above

* Module

| name         | version |
| ------------ | ------- |
| numpy        | 1.24.3  |
| sympy        | 1.11.1  |
| networkx     | 3.1     |
| mkl_random   | 1.2.4   |
| scipy        | 1.11.1  |
| matplotlib   | 3.7.2   |
| seaborn      | 0.12.2  |
| mpl_toolkits |         |
| warnings     |         |

> If we have matplotlib installed, we would be able to import mpl_toolkits directly.

* OS

> Mac OS X, Windows, or Linux

We use Anaconda GUI to run our code (which comes with the packages automatically installed). Otherwise, we may run `pip install` with the name and version for every candidate item.

### How to Obtain the Expressions and Figures

More detailed explanations are given in the comments and markdown notes (for ipython notebooks).

In particular, for every user-defined function, the corresponding docstring summarize its behavior and document its arguments.