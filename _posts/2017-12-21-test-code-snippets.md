---
layout: post
title: Building generations by Genetic algorithm
date: '2020-04-18'
desc: Building generations by Genetic algorithm
keywords: DATA SCIENCE
categories:
  - DATA SCIENCE
tags:
  - ''
  - Jekyll
icon: icon-DATA SCIENCE
---
> It is not the strongest of the species that survives, nor the most intelligent , but the one most responsive to change

Read it again cause the whole concept of Genetic algorithm lies in this line. The power of change makes things more valuable in this World.

By the name of Genetic algorithm you have much pretty idea how this algorithm works , Yes Genetic algorithms based on the ideas of natural selection and genetics. They are commonly used to generate high-quality solutions for optimization problems and search problems.

Genetic Algorithms were initially developed by John Holland , why the approach is so good in finding best solution for your query?
Image for post

Look above, here people are fighting with each other to show their capability and who’s the best among all of them. Just like this we compare our data to find the best output from millions of Data, so this is the most difficult job in Data Science , most of the algorithms are not able to give best solution and here comes the need of Genetic Algorithms or we can say the magic of nature . Genetic Algorithms are used when you wish to get “good solutions” for optimization problems “fast enough” which cannot be solved using the traditional algorithmic approaches.

Now what is optimization? — Optimization is the process of making something better or we can say finding the values of inputs in such a way that we get the “best” output values.

**GAs working**

In Genetic Algorithms, we have a population of possible solutions to the given problem. These solutions then undergo recombination and mutation (like in natural genetics), producing new children, and the process is repeated over various generations. Each individual (or candidate solution) is assigned a fitness value (based on its objective function value) and the fitter individuals are given a higher chance to mate and yield more “fitter” individuals. This is in line with the Darwinian Theory of “Survival of the Fittest”.


So now we are going through all the 6 steps of this diagram:

* Population
* Fitness function
* Parent Selection
* Crossover
* Mutation
* Survivor Selection

**1. Population**

Population is a subset of solutions in the current generation. It can also be defined as a set of chromosomes and a chromosome is one such solution to the given problem. A gene is one element position of a chromosome and Allele is the value a gene takes for a particular chromosome.
There are two population models widely in use −
Steady State — In steady state GA, we generate one or two off-springs in each iteration and they replace one or two individuals from the population. A steady state GA is also known as Incremental GA.
Generational — In a generational model, we generate ’n’ off-springs, where n is the population size, and the entire population is replaced by the new one at the end of the iteration.

**2. Fitness function**

Fitness function takes a candidate solution to the problem as input and produces as output how “fit” or how “good” the solution is with respect to the problem. After applying the fitness function, all the higher values of individual population (chromosome) are selected for matting pool for parent selection.

**3. Parent Selection**

Parent Selection is the process of selecting parents which mate and recombine to create off-springs for the next generation. Parent selection is very crucial to the convergence rate of the GA as good parents drive individuals to a better and fitter solutions.
There are four methods from which we can select the parents :
Fitness Proportionate Selection
Fitness Proportionate Selection is one of the most popular ways of parent selection. In this every individual can become a parent with a probability which is proportional to its fitness. Therefore, fitter individuals have a higher chance of mating and propagating their features to the next generation.
Tournament Selection
In tournament selection, we select “n” individuals from the population at random and select the best out of these to become a parent. The same process is repeated for selecting the next parent.
Rank Selection
It is used when the individuals in the population have very close fitness values.
Random Selection
In this strategy we randomly select parents from the existing population. There is no selection pressure towards fitter individuals and therefore this strategy is usually avoided.

**4. Crossover**

All selected parents are mate by crossover , in this more than one parent is selected and produce offspring using the genes of the parents.
And we have some of the most popularly used crossover operators that we are using for matting of parent.
One Point Crossover
In this a random crossover point is selected and the tails of its two parents are swapped to get new off-springs.
Image for post
#one point crossover
Multi Point Crossover
In Multi point crossover alternating segments are swapped to get new off-springs.
Image for post
Uniform Crossover
In a uniform crossover, we don’t divide the chromosome into segments, rather we treat each gene separately.
Image for post

**5. Mutation**

In biology a mutation is a change that occurs in our DNA sequence, it is like adding new value in previous solutions. In mutation, the solution may change entirely from the previous solution.It is used to maintain and introduce diversity in the genetic population and is usually applied with a low probability. If the probability is very high, the GA gets reduced to a random search. click here to know more about mutation.

**6. Survivor Selection**

The Survivor Selection selects which individuals are to be kicked out and which are to be kept in the next generation.
There are two strategies widely used:
Age Based Selection — The oldest members of the population (max age) are kicked out of the population no matter how good its fitness is and the ages of the rest of the members are incremented by one.
Fitness Based Selection — In this fitness based selection, the children tend to replace the least fit individuals in the population.

**Closure**

We have learned how we can get one perfect solution from millions of choices .
In my next article I will implement all these steps in coding so as to get more idea how computer does genetic algorithm.
Hope after reading it, it has become your favourite algorithm like me😄
Connect with me:
LinkedIn: http://linkedin.com/in/monika0104