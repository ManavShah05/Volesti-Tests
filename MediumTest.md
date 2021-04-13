
> Add counters in C++ code of volesti to count the average number of reflections per HMC step. For different (a) integration time, (b) step length in ODE solver, 
(c) dimension, compute the PSRF/run-time and Effective Sample Size (ESS)/run-time for a large number of samples and report.

### 1. Adding run time counter

#### Code:
> I added the following code in int main() of simple_hmc.cpp

![Screenshot from 2021-04-12 18-07-06](https://user-images.githubusercontent.com/71564257/114481992-99b60f80-9bba-11eb-9a8d-3e7df57e4ad1.png)

#### Output:
```
Step size (final): 0.234793
Discard Ratio: 0.02
Average Acceptance Log-prob: 0.978655
+ Run time: 0.231689 s
```

### 2. Finding the Effective Sample Size

#### Formula:
![Image](https://sawtoothsoftware.com/help/lighthouse-studio/manual/effective_sample_size.png)

In this program all the data points have an equal weight due to which n effective will be equal to n. 
