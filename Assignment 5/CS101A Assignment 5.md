# CS101A Assignment 5

> 11510225 Yuxing Hu (胡与兴)

### Question 1: Turing machine

 (a) Please write down the sequence of configurations

​	(1) 10#0#

```
(q1)10#0#
x(q3)0#0#
x0(q3)#0#
x0#(q5)0#
x0#(qreject)0#
```

​	(2) 01#00

```
(q1)01#00
x(q2)1#00
x1(q2)#00
x1#(q4)00
x1(q6)#x0
x(q7)1#x0
(q7)x1#x0
x(q1)1#x0
xx(q3)#x0
xx#(q5)x0
xx#x(q5)0
xx#x(qreject)0
```

(b) Is A a Turing-recognizable language?  **Yes.**

Is A a Turing-decidable language? **Yes.**

### Question 2:  Prove (𝒏+𝒂)^𝒃 =𝑶(𝒏^𝒃)

```
(n + a)^ b ≥ (n − |a|)^ b, where n > 0
          ≥ ((c2′)n)^ b for c2′ = 1/2 where n ≥ 2|a|
            as n/2 ≤ n − |a|, for n ≥ 2|a|
Thus
(n + a)^b = O(n^b)
```

### Question 3: Rank the functions

g1 = 666log2(n^3); g2 = 0.0001n; g3 = 10log2√n); g4 = n^(1.01)