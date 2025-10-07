---
title: Mersenne primes and their exponents
author: Killian O'Brien
date: October 2025
---

In the previous lecture we discussed (and typeset) the proof that there are an infinite number of prime numbers. 

Despite knowing that there are an infinite number of primes, of course humans have only been able to identify a finite collection of primes so far. Generally, the larger an integer is, the harder it is to check whether it is prime or not. Since 1996 the largest known primes to humans have all been found by the [GIMPS](https://www.mersenne.org/primes/){target="_blank"}.

At the time of writing, the largest known prime to humans is the integer 
$$2^{136,279,841} - 1,$$
a number with over 41 million digits when written out fully in the usual base-10 manner. This is an example of what is known as a *Mersenne prime*, a prime number which is one less that a power of $2$. 

In fact, the exponent there, $136,279,841$ is itself a prime number. This is not surpising, thanks to the following theorem. 

**Theorem**: *If the number $2^n -1$ is prime, then the exponent $n$ is also prime*. 

This theorem can be proved using a relatively short factorisation argument. We normally prove the equivalent *contra-postive* statement:

**Theorem**: *If the number $n$ is composite, then associated Mersenne number $2^n -1$ is also composite.*

Try to obtain an argument that proves this theorem, and type it up using $\LaTeX$. If you are struggling to make progress you could do some internet searching. Here is a hint. Assume the number $n$ is composite, i.e. $n$ can be factorised as 
$$n = rs,$$
for a pair of integers $r$ and $s$ with $1 \lt r$ and $1 \lt s$. 
Now try to construct a factorisation of the Mersenne number, which will show that it is composite. The central part of the argument starts with 
$$2^n - 1 = 2^{rs} - 1 = \left ( 2^r \right )^s - 1^s = \dots ,$$
and continue by using a stanard polynomial factorisation result for the difference of powers. 