# Simulation & Modeling Sessional
# CSE424

# Group 3
1. Devesh Biswas (CSE 01406300) [Team Leader]

2. Reaz Uddin Munna (CSE 01406368)

3. Nusrat jahan (CSE 01406348)

4. Md.Moinuddin (CSE 01406315)

5. Rahat Alam (CSE 01406358)

# Course Instructor:
Mr. Muhtadir Rahman

Lecturer, 

Department of CSE

Port City International University

# Single channel queue system

# Introduction:
The single channel queuing model can be fitted in situations where the following seven conditions are fulfilled: The number of arrivals per unit of time is described by Poisson distribution. The mean arrival rate is denoted by λ. 
 single-channel queuing:
			A queue can be thought of as nearly a black box. Jobs or "customers" arrive to the queue, possibly wait some time, take some time being processed, and then depart from the queue.
			
			
![im1](https://user-images.githubusercontent.com/81485746/113812748-6f1a2000-9790-11eb-91d5-2a75004dce7f.PNG)
			

		


		a black box. Jobs or "customers" arrive to the queue

The single channel queuing model can be fitted in situations where the following seven conditions are fulfilled: The number of arrivals per unit of time is described by Poisson distribution. The mean arrival rate is denoted by λ. The service time has exponential distribution.

# Continuous  probability distribution:
A probability distribution in which the random variable X can take on any value (is continuous). Because there are infinite values that X could assume, the probability of X taking on any one specific value is zero. ... The normal distribution is one example of a continuous distribution.

The probability that a particular random variable will equal a certain value is zero. For example, let's say you had a continuous probability distribution for men's heights. ... The chart shows that the average man has a height of 70 inches (50% of the area of the curve is to the left of 70, and 50% is to the right)
A continuous distribution describes the probabilities of the possible values of a continuous random variable. A continuous random variable is a random variable with a set of possible values (known as the range) that is infinite and uncountable.
Probabilities of continuous random variables (X) are defined as the area under the curve of its PDF. Thus, only ranges of values can have a nonzero probability. The probability that a continuous random variable equals some value is always zero.

# Discrete probability distribution:

A discrete distribution describes the probability of occurrence of each value of a discrete random variable. A discrete random variable is a random variable that has countable values, such as a list of non-negative integers.
With a discrete probability distribution, each possible value of the discrete random variable can be associated with a non-zero probability. Thus, a discrete probability distribution is often presented in tabular form.
There are many discrete probability distributions to be used in different scenarios. We will discuss Discrete distributions in this post. Binomial and Poisson distributions are the most discussed ones in the following list-
1.Bernoulli Distribution
2.Binomial Distribution
3. Hypergeometric Distribution
4.Negative Binomial Distribution
5.Geometric Distribution
6.Poisson Distribution
7.Multinomial Distribution


# Discrete random variable:
A random variable is a numerical quantity that is generated by a random experiment.
A discrete random variable is one which may take on only a countable number of distinct values such as 0,1,2,3,4,........ Discrete random variables are usually (but not necessarily) counts. If a random variable can take only a finite number of distinct values, then it must be discrete. Examples of discrete random variables include the number of children in a family, the Friday night attendance at a cinema, the number of patients in a doctor's surgery, the number of defective light bulbs in a box of ten.
The probability distribution of a discrete random variable is a list of probabilities associated with each of its possible values. It is also sometimes called the probability function or the probability mass function.

(Definitions taken from Valerie J. Easton and John H. McColl's Statistics Glossary v1.1)

Example:
Suppose a variable X can take the values 1, 2, 3, or 4.
The probabilities associated with each outcome are described by the following table:

![im2](https://user-images.githubusercontent.com/81485746/113810132-6246fd80-978b-11eb-90db-96f68c25f5fd.gif)

	Outcome 	1	2	3	4
	Probability	0.1	0.3	0.4	0.2
The probability that X is equal to 2 or 3 is the sum of the two probabilities: P(X = 2 or X = 3) = P(X = 2) + P(X = 3) = 0.3 + 0.4 = 0.7. Similarly, the probability that X is greater than 1 is equal to 1 - P(X = 1) = 1 - 0.1 = 0.9, by the complement rule.
This distribution may also be described by the probability histogram shown to the right:


# Continuous random variable:
A continuous random variable is one which takes an infinite number of possible values. Continuous random variables are usually measurements. Examples include height, weight, the amount of sugar in an orange, the time required to run a mile.
A continuous random variable is not defined at specific values. Instead, it is defined over an interval of values, and is represented by the area under a curve (in advanced mathematics, this is known as an integral). The probability of observing any single value is equal to 0, since the number of values which may be assumed by the random variable is infinite.
Suppose a random variable X may take all values over an interval of real numbers. Then the probability that X is in the set of outcomes A, P(A), is defined to be the area above A and under a curve. The curve, which represents a function p(x), must satisfy the following:
1: The curve has no negative values (p(x) > 0 for all x)
2: The total area under the curve is equal to 1.
A curve meeting these requirements is known as a density curve.
(Definition taken from Valerie J. Easton and John H. McColl's Statistics Glossary v1.1)
Example
The cumulative distribution function for the above probability distribution is calculated as follows:
The probability that X is less than or equal to 1 is 0.1,
the probability that X is less than or equal to 2 is 0.1+0.3 = 0.4,
the probability that X is less than or equal to 3 is 0.1+0.3+0.4 = 0.8, and
the probability that X is less than or equal to 4 is 0.1+0.3+0.4+0.2 = 1.

![im3](https://user-images.githubusercontent.com/81485746/113810129-61ae6700-978b-11eb-997a-52b0049f8dd2.gif)

The probability histogram for the cumulative distribution of this random variable is shown to the right:

# Probability distribution:
The probability distribution gives the possibility of each outcome of a random experiment. It provides the probabilities of different possible occurrences.
If two coins are tossed, then the probability of getting 0 heads is ¼, 1 head will be ½ and both heads will be ¼. So, the probability P(x) for a random experiment or discrete random variable x, is distributed as:
P(0) = ¼
P(1) = ½
P(2) = 1/4
P(x) = ¼ + ½ +¼ = 1

One way is that you visualize the grades and see if you can find a trend in the data.


 ![im4](https://user-images.githubusercontent.com/81485746/113810127-607d3a00-978b-11eb-8f79-3eb2b7a4d16a.png)
 


# Importance of  random number generation:

The standard random number generator you've got (rand() in C after a simple transformation, equivalents in many languages) is a fairly good approximation to a uniform distribution over the range [0,1]. If that's what you need, you're done. It's also trivial to convert that to a random number generated over a somewhat larger integer range.
Conversion of a Uniform distribution to a Normal distribution has already been covered on SO, as has going to the Exponential distribution.
[EDIT]: For the triangular distribution, converting a uniform variable is relatively simple (in something C-like):
double triangular(double a,double b,double c) {
   double U = rand() / (double) RAND_MAX;
   double F = (c - a) / (b - a);
   if (U <= F)
      return a + sqrt(U * (b - a) * (c - a));
   else
      return b - sqrt((1 - U) * (b - a) * (b - c));
}
That's just converting the formula given on the Wikipedia page. If you want others, that's the place to start looking; in general, you use the uniform variable to pick a point on the vertical axis of the cumulative density function of the distribution you want (assuming it's continuous), and invert the CDF to get the random value with the desired distribution.
The right way to do this is to decompose the distribution into n-1 binary distributions. That is if you have a distribution like this:
A: 0.05
B: 0.10
C: 0.10
D: 0.20
E: 0.55
You transform it into 4 binary distributions:
1. A/E: 0.20/0.80
2. B/E: 0.40/0.60
3. C/E: 0.40/0.60
4. D/E: 0.80/0.20
Select uniformly from the n-1 distributions, and then select the first or second symbol based on the probability if each in the binary distribution.

It actually depends on distribution. The most general way is the following. Let P(X) be the probability that random number generated according to your distribution is less than X.
You start with generating uniform random X between zero and one. After that you find Y such that P(Y) = X and output Y. You could find such Y using binary search (since P(X) is an increasing function of X).
This is not very efficient, but works for distributions where P(X) could be efficiently computed.

Properties of random variables:
		 A random variable is a process for choosing a random number. A continuous random variable is defined by a probability density function p(x), with these properties: p(x) ≥ 0 and the area between the x-axis and the curve is 1: ∫ -∞ ∞ p(x) dx = 1.


1.	A random variable is a process for choosing a random number.
 
2.	A discrete random variable is defined by its probability distribution function:
 
Outcome	Probability
x1	p1
x2	p2
⋮	⋮
xn	pn
3.	
The probabilities of a discrete random variable must sum to 1:
 
4.	E(x) = Σi=1n pi

Properties:
For properties 1 to 7, c is a constant; x and y are random variables.
1.	E(x + y) = E(x) + E(y).
 
2.	E(cx) = c E(y).
 
3.	Var(x) = E(x2) - E(x)2
 
4.	If x and y are independent, then Var(x + y) = Var(x) + Var(y).
 
5.	Var(x + c) = Var(x)
 
6.	Var(cx) = c2 Var(x)
 
7.	Cov(x + c, y) = Cov(x, y)
 
8.	Cov(cx, y) = c Cov(x, y)
 
9.	Cov(x, y + c) = Cov(x, y)
 
10.	Cov(x, cy) = c Cov(x, y)
 
11.	If x1, x2, ..., xn are independent and N(μ, σ2), then E(x) = μ. We say that x is unbiased for μ.
 
12.	If x1, x2, ... , xn are independent and N(μ, σ2), then E(s) = σ2.   We say that s is unbiased for σ2.
For properties 8 to 12, w and v are random vectors; b is a constant vector; A is a constant matrix.
8.	E(v + w) = E(v) + E(w)
 
9.	E(b) = b
 
10.	E(Av) = A E(v)
 
11.	Cov(v + b) = Cov(v)
 
12.	Cov(Av) = A Cov(v) AT
 



# Why inter arrival time is Poission distributed:


Because These “interarrival” times are typically exponentially distributed. If the mean interarrival time is 1/λ (so λ is the mean arrival rate per unit time), then the variance will be 1/λ2 (and the standard deviation will be 1/λ).

The above construction can be made mathematically rigorous. The resulting random process is called a Poisson process with rate (or intensity) λλ. Here is a formal definition of the Poisson process.
# The Poisson Process

Let λ>0λ>0 be fixed. The counting process {N(t),t∈[0,∞)}{N(t),t∈[0,∞)} is called a Poisson process with rates λλ if all the following conditions hold:
N(0)=0N(0)=0;
N(t)N(t) has independent increments;
the number of arrivals in any interval of length τ>0τ>0 has Poisson(λτ)Poisson(λτ) distribution.
Note that from the above definition, we conclude that in a Poisson process, the distribution of the number of arrivals in any interval depends only on the length of the interval, and not on the exact location of the interval on the real line. Therefore the Poisson process has stationary increments.


Let N(t)N(t) be a Poisson process with rate λλ. Let X1X1 be the time of the first arrival. Then,
P(X1>t)=P(no arrival in (0,t])=e−λt.P(X1>t)=P(no arrival in (0,t])=e−λt.
We conclude that
FX1(t)=⎧⎩⎨⎪⎪1−e−λt0t>0otherwiseFX1(t)={1−e−λtt>00otherwise
Therefore, X1∼Exponential(λ)X1∼Exponential(λ). Let X2X2 be the time elapsed between the first and the second arrival (Figure 11.4).
 Figure 11.4 - The random variables X1X1, X2X2, ⋯⋯ are called the interarrival times of the counting process N(t)N(t).
Let s>0s>0 and t>0t>0. Note that the two intervals (0,s](0,s] and (s,s+t](s,s+t] are disjoint. We can write
P(X2>t|X1=s)=P(no arrival in (s,s+t]|X1=s)=P(no arrivals in (s,s+t])(independent increments)=e−λt.P(X2>t|X1=s)=P(no arrival in (s,s+t]|X1=s)=P(no arrivals in (s,s+t])(independent increments)=e−λt.
We conclude that X2∼Exponential(λ)X2∼Exponential(λ), and that X1X1 and X2X2 are independent. The random variables X1X1, X2X2, ⋯⋯ are called the interarrival times of the counting process N(t)N(t). Similarly, we can argue that all XiXi's are independent and Xi∼Exponential(λ)Xi∼Exponential(λ) for i=1,2,3,⋯i=1,2,3,⋯.


# Interarrival Times for Poisson Processes

If N(t)N(t) is a Poisson process with rate λλ, then the interarrival times X1X1, X2X2, ⋯⋯ are independent and
Xi∼Exponential(λ), for i=1,2,3,⋯.Xi∼Exponential(λ), for i=1,2,3,⋯.
Remember that if XX is exponential with parameter λ>0λ>0, then XX is a memoryless random variable, that is
P(X>x+a|X>a)=P(X>x), for a,x≥0.P(X>x+a|X>a)=P(X>x), for a,x≥0.
Thinking of the Poisson process, the memoryless property of the interarrival times is consistent with the independent increment property of the Poisson distribution. In some sense, both are implying that the number of arrivals in non-overlapping intervals are independent. 


![im5](https://user-images.githubusercontent.com/81485746/113810136-63782a80-978b-11eb-8cf1-2dc43eebb0bf.png)





 



# Why service time is exponentially  distributed:

Because G, which stands for general service time distribution. M, which stands for memoryless (or exponential) interarrival time or service time distribution.
 Note that an exponentially distributed interarrival time means that customers arrive according to a Poisson process.
While studying waiting lines, where jobs wait for processing or service, the model must account for random variation in the processing/service time. The exponential distribution is often a good approximation of service time. If so, the variance of exponential service times is usually much wider than other distributions, such as the normal distribution. The existence of exponentially distributed times should not be assumed, but should be tested by chi-squared tests, or other statistical methods for identifying probability distributions.
Copyright information
© Kluwer Academic Publishers 2000

# Motivation is solven single queueing channel problem:


# Code result output:

![im6](https://user-images.githubusercontent.com/81485746/113810134-62df9400-978b-11eb-984a-0160f7dd23c9.jpg)

 

# Matcha.io:
# Table:
# Conclusion:
The single channel queuing model referred above, is the most simple model which is based on the above mentioned assumptions. However, in reality, there are several limitations of this model in its applications. One obvious limitation is the possibility that the waiting space may in fact be limited. Another possibility is that arrival rate is state dependent. That is, potential customers are discouraged from entering the queue if they observe a long line at the time they arrive. Another practical limitation of the model is that the arrival process is not stationary.
