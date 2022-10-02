# Concession-period-optimization
The code for the optimization of concession period of PPP projects
Input: The primary parameters, i.e., initial investment, equity structure parameters;
Output: Ip, Io, the optimal concession period T;

1 if the project is acceptable do
2     if NPVt1 >= 0 for the private developer do
3             calculate the NPV value for the private developer
4             calculate the option value for the private developer
5             calculate the NPV value for the owner
6             calculate the option value for the owner
7         return Ip, Io;
8     collect all Ip, Io into a list
9     applying Non-dominated sorting rule
10     return rank 1 tier, i.e., the Pareto front
11 determine the final optimal solution and the corresponding concession T, according to the knee point rule
