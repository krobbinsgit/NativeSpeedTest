# NativeSpeedTest
Investigation of how fast/slow anneals change solution quality on hardware native problems

# Plots to make
* Probability of obtaining optimal solution as a function of anneal time. Requires preselected problems of a fixed size and that the problems are easily calculable beforehand.
* Best solution value for a given problem as a function of anneal time. Requires preselected problems of a fixed size.
* Once I find a "good" problem (hopefully I'll know what that means when I see it) I can vary interaction strengths as well to see if that matters.

# Problem Types
I want the problems to be hardware native. The issue is that there isn't a "generic" problem I can do... should I just stick with ```ran-k``` problems?
* Start with a very basic problem: antiferromagnetic chain of length 2, interaction strength the same, and see if I can break it at any speeds. After that try with the frustrated antiferromagnetic case of N=3 and cyclic.
* Antiferromagnetic w/ strong bonds: $N$-spin chain with $h$ values set to $\pm 1$ (alternating) and $J$ values set to $-1$. Cyclic or no? *Should be exactly solvable.*
* ```ran-k``` will create random problems. There is no easy way to consistently compare solutions though... unless I modify to ensure problem belongs to exactly-solvable class, maybe.
* Same antiferromagnetic problem as bullet point 2 but 2D lattice instead of a chain. Cyclic or no?

