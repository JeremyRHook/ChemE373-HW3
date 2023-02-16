# ChemE375-HW3
# ChemE 375: HW3

The assignment is due midnight **before** the beginning of the next class period.

Note: Use Excel for all problems.  Remember that on all Excel assignments, **some points will be given for following the recommended practice of naming variables and for presentation (formatting)**.  For each problem please use a separate worksheet and highlight your answers!

## Problem 1

Heart rate data (Beats per minute or BPM) as a function of time (sec) for a twenty-minute period of constant exertion is found in the "Problem 1" worksheet of the workbook. The time of each measurement, in seconds, is listed in Column A, and the measured heart rate, in beats per minute, is found in Column B. Using Excel,

1. Determine the values of c0, c1, c2, and c3 that result in the best fit of the data to the following equation:

<a href="https://www.codecogs.com/eqnedit.php?latex=BPM&space;=&space;c_0&space;&plus;&space;c_1t&space;-&space;c_2e^{-c_3t}" target="_blank"><img src="https://latex.codecogs.com/gif.latex?BPM&space;=&space;c_0&space;&plus;&space;c_1t&space;-&space;c_2e^{-c_3t}" title="BPM = c_0 + c_1t - c_2e^{-c_3t}" /></a>

2. Plot the raw data and data generated using the approximating function above (BPM) vs time (sec).
3. Calculate the R2 valued for the fit. Is the fit good?

* Providing good guess values is the key to getting this fit to solve.
* To verify you have solved correctly or obtained good guess values, plot the data and the function before you try to solve using Solver.
* Think about how large each constant should be based on what it is multiplied by.
* You should get an R2 value >0.98.

## Problem 2

The worksheet "Problem 2" contains data for the response for a first-order system with time delay. Such data is used to create control devices to keep operations running correctly.

1. Find the constants θ and τ in the equation

<a href="https://www.codecogs.com/eqnedit.php?latex=y(t)&space;=&space;5\bigg[&space;1&space;-&space;e^{-\frac{(t&space;-&space;\theta)}{\tau}}&space;\bigg]S(t&space;-&space;\theta)" target="_blank"><img src="https://latex.codecogs.com/gif.latex?y(t)&space;=&space;5\bigg[&space;1&space;-&space;e^{-\frac{(t&space;-&space;\theta)}{\tau}}&space;\bigg]S(t&space;-&space;\theta)" title="y(t) = 5\bigg[ 1 - e^{-\frac{(t - \theta)}{\tau}} \bigg]S(t - \theta)" /></a>

where

<a href="https://www.codecogs.com/eqnedit.php?latex=S(t&space;-&space;\theta)&space;=&space;\begin{cases}&space;0,&&space;t<\theta\\&space;1,&space;&&space;t&space;\ge&space;\theta&space;\end{cases}" target="_blank"><img src="https://latex.codecogs.com/gif.latex?S(t&space;-&space;\theta)&space;=&space;\begin{cases}&space;0,&&space;t<\theta\\&space;1,&space;&&space;t&space;\ge&space;\theta&space;\end{cases}" title="S(t - \theta) = \begin{cases} 0,& t<\theta\\ 1, & t \ge \theta \end{cases}" /></a>

best fit the process data y(t).

2. Make a graph showing the data (as points) and the fit (as a line).
3. Determine the R2 value of the fit.
4. Which of the functions available with Excel's Trendline feature best fit the data? How many constants are used to achieve this fit? What is its R2 value?

## Problem 3

In Worksheet "Problem 3" create 1000 random numbers with a Poisson distribution using a lambda of 1. Using bins (0,1,2,3,4,5) determine the frequency at which a number appears and plot this with a column plot (frequency vs. bin).

## Problem 4

A first-order reaction governed by A --> B has rate

<a href="https://www.codecogs.com/eqnedit.php?latex=\frac{dC_A}{dt}&space;=&space;-kC_A" target="_blank"><img src="https://latex.codecogs.com/gif.latex?\frac{dC_A}{dt}&space;=&space;-kC_A" title="\frac{dC_A}{dt} = -kC_A" /></a>

where C_A is the concentration (kmol/m^3), t is time, and k is a rate constant. The initial concentration is C_A0 (5 kmol/m^3) and k=1 s^-1.

1. Solve for C_A(t) two ways: (1) analytically by separating variables and integrating; (2) using the Explicit Euler method. For the Euler method, evaluate the rate (RHS) at time n, then solve the whole equation for values at time n+1.

<a href="https://www.codecogs.com/eqnedit.php?latex=\frac{dC_A}{dt}&space;\approx&space;\frac{C_A_{n&plus;1}&space;-&space;C_A_{n}}{\Delta&space;t}" target="_blank"><img src="https://latex.codecogs.com/gif.latex?\frac{dC_A}{dt}&space;\approx&space;\frac{C_A_{n&plus;1}&space;-&space;C_A_{n}}{\Delta&space;t}" title="\frac{dC_A}{dt} \approx \frac{C_A_{n+1} - C_A_{n}}{\Delta t}" /></a>

Plot the two versions of C_A(t) on the same plot. Label and format the plot including axis labels and legends etc. so you can clearly communicate the solution. Use a time step size of Δt=0.5 s and plot to t_end = 7s (14 steps).

2. Compare the curves. Why are they different?
3. Copy the figure and paste as an image in the same document. Change Δt from 0.5 to 1.5. Copy the figure as an image again. Change Δt to 2.1. Comment on the three plots.

## Problem 5

We are performing a chemical reaction as follows:

A + B --> C (Reaction 1)
B + C --> D (Reaction 2)

Product C is desired, but as soon as C is formed, some B reacts with it to form the undesired D.

The rate of change of the concentrations of each of the species is given by

<a href="https://www.codecogs.com/eqnedit.php?latex=\frac{dA}{dt}&space;=&space;-k_1&space;AB" target="_blank"><img src="https://latex.codecogs.com/gif.latex?\frac{dA}{dt}&space;=&space;-k_1&space;AB" title="\frac{dA}{dt} = -k_1 AB" /></a>

<a href="https://www.codecogs.com/eqnedit.php?latex=\frac{dB}{dt}&space;=&space;-k_1&space;AB&space;-&space;k_2&space;BC" target="_blank"><img src="https://latex.codecogs.com/gif.latex?\frac{dB}{dt}&space;=&space;-k_1&space;AB&space;-&space;k_2&space;BC" title="\frac{dB}{dt} = -k_1 AB - k_2 BC" /></a>

<a href="https://www.codecogs.com/eqnedit.php?latex=\frac{dC}{dt}&space;=&space;k_1&space;AB&space;-&space;k_2&space;BC" target="_blank"><img src="https://latex.codecogs.com/gif.latex?\frac{dC}{dt}&space;=&space;k_1&space;AB&space;-&space;k_2&space;BC" title="\frac{dC}{dt} = k_1 AB - k_2 BC" /></a>

<a href="https://www.codecogs.com/eqnedit.php?latex=\frac{dD}{dt}&space;=&space;k_2&space;BC" target="_blank"><img src="https://latex.codecogs.com/gif.latex?\frac{dD}{dt}&space;=&space;k_2&space;BC" title="\frac{dD}{dt} = k_2 BC" /></a>

The initial concentrations are A_0=1, B_0=1, C_0=1, D_0=0. Also, k_1=1 L/mol*s and k_2=1.5 L/mol*s.

1. Solve for the concentrations of A, B, C, and D as functions of time. Use a time step size of dt=0.2s and solve to t=3 s. Also solve for the selectivity defined as S=C/(C+D) as a function of time. (S. is initially undefined, but you can set it equal to 1 at t=0). Use Euler's equation applied to each species above.

2. Plot the concentrations of A, B, C, D and S as functions of time on the same plot. Label the axes as "time (s)" and "concentration (mol/L)"

3. What is the final value of the selectivity?

4. Assuming the values of C_0, D_0, k_1, and k_2 are fixed, how can you increase the final value of the selectivity given the above reactions?
