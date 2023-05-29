A\. Explanation of the part in the code written by us: 
The part we added to the code is the implementation of the simulated annealing
process using the while loop. The loop generates neighbour solutions by flipping
the selection of items, evaluates their value and then decides whether
to accept them according to the acceptance probability. This process
continues until the temperature reaches a considered low value, pointing
convergence. The best solution found throughout the iterations is kept
and printed at the end. We also made some additions so that we can
observe the execution time for Q1 using "java.lang.System" package.

B\. Answers to the questions given:

1\. How does the execution time change when the cooling rate is
increased?

We ran the code with multiple cooling rates with a fixed rng seed after
making the modifications we made to the code so that we can observe the
cooling rate and our conclusions are as follows:

 - The execution time of simulated annealing depends on the number of
iterations performed. The cooling rate affects how quickly the
temperature decreases, which in turn affects the convergence rate of the
algorithm.  
- A higher cooling rate means faster convergence, which
means that less iterations are required to find a solution. But, a
higher cooling rate may also require more iterations to achieve the
desired solution quality.  
- The relationship between cooling rate and
execution time is neither black nor white. It is possible that a higher
cooling rate can lead to faster and slower execution times, depending on
the problem.

In conclusion, our observations showed us that increasing the cooling
rate can both increase and decrease the execution time.

2\. How does the execution time and solution quality change when the
difference between starting temperature and stopping temperature is
increased?

We ran the code with multiple initial temperatures with a fixed rng seed
after making the modifications we made to the code so that we can
observe the cooling rate and our conclusions are as follows:

 - When the temperature difference increases, the execution time usually
increases.  
- A larger temperature difference means more exploration in
the first stages of the annealing process, which can increase the time
required to converge to the optimal solution.  
- But, a larger temperature difference also means a wider exploration range, possibly
leading to better solution.  
- It's essential to balance by choosing an
appropriate temperature difference based on the problem details and
desired solution quality.
