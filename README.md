#  Simulation & Modeling Sessional
#  CSE-424


#  Group 02 
#       1. Devesh Biswas (CSE-01406300) 
#       2. Reaz Uddin Munna (CSE-01406368) 
#       3. Md.Moinuddin (CSE-01406315) 
#       4. Nusrat Zahan (CSE-01406348)
#       5. Rahat Alam (CSE-01406358) 



# Problem:
# Single-Channel-Queue-System


# Background:
Random numbers are very important in discrete event simulation for generating event times. A chain of
random numbers must hold two major properties-1) Uniformity 2) Independence. A stochastic simulation model
requires one or more random variable as inputs. The random numbers can be generated from a random variable say X.
P(X=x) is greater than zero and ranges between zero and one when the total number of possible outcomes is finite. In
such a case, the random variable X is said to be discrete. P(X=x) is exactly zero when the total number of possible
outcomes is infinite. In such a case, the random variable X is said to be continuous. So, in our study, we have now
found two terms- Discrete Random Numbers and Continuous Random Numbers. There are many techniques to
generate random numbers such as- Linear Congruential Method, Combined Linear Congruential Method etc. These
generators can also be used to generate “seed” of a Random-Number streams since, generators tend to have repeats
to a certain extent. But, in practice, a simulation analyst might not deal with random number generators or streams
directly because of their insufficiency in usability, though they pass two important tests-1) Frequency Test and 2)
Autocorrelation Test. Still some underlying patterns that might be taken into considerations. Once we have accepted a
good random number generator that passes those two tests to assure its two attributes that is U[0,1)

and independence, now we can switch to other distributions like Poisson, Exponential, Normal/Gaussian, Truncated Normal, Gamma and Weibull distribution and generate random variates from their probability density function(pdf). That means, random numbers are employed in generating random variates. Most common methods for generating random variates are- 1) Inverse Transform Technique, 2) Acceptance-Rejection Technique, and 3) Special Properties. Inverse Transform Technique is the underlying policy for sampling from an extensive family of discrete distribution.


# Problem Statement
Now, simulate this bank problem having µ=5.6 customers/minute (arrival rate) and λ=5 customers/minute (service rate) for 20 customers. You should use exactly 19 to 20 random variates for generating the random variables(two). You don’t need to consider after precision values of decimal point for service times during simulation for the convenience. You can use any subroutine, object, or any built-in function of any relevant programming language. The average number of customer waiting, the average waiting time of a customer should be your statistical estimators for examining the true characteristics of the system.
