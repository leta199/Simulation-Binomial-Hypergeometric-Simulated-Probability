# Binomial vs Hypergeometric vs  Simulated Probability 
Uncovering how binomial, hypergeometric and simulated probability compare when picking red balls in a sample from a large population.

This project aims to create an experiment that can simulate binomial and hypergeometric probavikites using stochastic methods and determine the level of precision and accuracy that can be generated. 

This notebook will:

- Use `pbinom` and `phyper` function to aproximate probability.
- Approximate probavility in question using stochastic approximation in base R.

## HOW IT'S MADE 
Languages used: R (version 4.5.1)    
Environement: RStudio 

[![Language: R](https://img.shields.io/badge/Language-R-276DC3.svg?style=flat-square)](https://www.r-project.org/)
[![Built with RStudio](https://img.shields.io/badge/IDE-RStudio-75AADB?style=for‐the‐badge&logo=rstudio&logoColor=white)](https://www.rstudio.com/)
![Status](https://img.shields.io/badge/Status-Completed-lightgrey)

## METHODS AND TECHNIQUES  
**Binomial and Hypergeometric probability**   
The new funcions: `pbinom()` and `phyper()` are new functions I learned how to use to calculate the left tail probability.   
`pbinom()`- utilises the threshhold for our red balls left tail  proability , sample size and probaility of success.   
`phyper()`- utilises the threshhold for our red balls left tail probability, number of red balls, number of non-red balls and sample size. 

**Setup of simulation**     
`set.seed()`- to enire reproducibility.   
Define our population sizes and number of repetitions in each experiment.   
Create a length = 4 vector to store probability. 

**For loop**  
Defining the counter for the outer for loop.     
Partitioning the balls into red and non-red for each population. 
Creating our sample size and randomly selecting balls from population with `sample()`.   
Assigning 1 if red balls are equal to or less than 0.02*n red balls and 0 if not.   
Assing the average of 5000 repititions to overall probability. 

## VISUALISATIONS 

**Dataframe**   
Created to compare the values of probabilites with each function and the simulation.  
<img width="480" height="109" alt="Image" src="https://github.com/user-attachments/assets/c7dad1fa-7a27-4f88-b6bd-bc07a47d961a" />

**Line graph**   
Shows how our probability changes between each method that we use to calculate probability. 
<img width="1440" height="874" alt="Image" src="https://github.com/user-attachments/assets/f5d17a2a-14fe-4ced-b64b-03e1148721d7" />

 ## PROJECT STRUCTURE   
 
|[Simulation Binomial Hypergoemetric Simulated Probability](https://github.com/leta199/Simulation--Binomial-Hypergeometric-Simulated-Probability-)     
|├──[Table of comparison](https://github.com/leta199/Simulation--Binomial-Hypergeometric-Simulated-Probability-/blob/main/Binom%20vs%20Hyper%20vs%20Sim%20.png)  
|├──[Compiled pdf](https://github.com/leta199/Simulation--Binomial-Hypergeometric-Simulated-Probability-/blob/main/Binom-vs-Hyper-vs-Sim.pdf)        
|├──[Binom vs Hyper vs Simulation (R)](https://github.com/leta199/Simulation--Binomial-Hypergeometric-Simulated-Probability-/blob/main/Binomial%20vs%20Hypergeomtric%20vs%20Sim.r)  
|└── [README](https://github.com/leta199/Simulation--Binomial-Hypergeometric-Simulated-Probability-/blob/main/README.md)  

## AUTHORS   
[leta199](https://github.com/leta199)  

