---
title: Hw2
author: Jessica Jones
partner: Alexa Fernando, Christine Ramos
date: 1/28/2019
---

In the report, complete the following.
- Explain the objective of the problem.
- Give your solution.
- Include all your project codes in the [codes/assg](../../codes/assg) folder,
  if required.
- Explain your code snippets, if required.
- Include screenshots of the simulations in this folder, and insert them into
  the markdown file, if required.
- Explain why the simulations are correct, if required.

You can embed math equations into Github Markdown file using a [web service](https://www.codecogs.com/latex/eqneditor.php)

## (5 pts)
Describe the concept known as Moore’s Law.

The objective of the problem is to demonstrate your knowledge of the concept of Moore’s law.

Moore’s law is an idea introduced by Gordon Moore, the co-founder of Intel, in 1965. Moore’s law is the notion that in about 18 months, the number of transistors on a chip doubles (or the amount of space a transistor takes up is halved). It is not necessarily a scientific law but an industry standard; this law was always eventually going to expire because of limitations of the materials used and the laws of physics. 

## (5 pts)
Describe the behavior of the CMOS transistor
circuit shown below, clearly indicating
when the transistor circuit conducts.

![](figures/problem_2.png)

The objective of the problem is to demonstrate your knowledge of a CMOS.
This CMOS uses two PMOS (positive polarity) circuits which conduct when a positive voltage is applied. Since the circuit uses only PMOS, it will only conduct when a positive voltage is applied.  


## (5 pts)
If we apply a voltage to the gate of a CMOS transistor, why doesn’t the current flow
to the transistor’s source or drain?

The objective of the problem is to show your understanding of how a CMOS works.

If the voltage is negative, it will not attract electrons between its source and drain, which allows the transitor to conduct. (see next question)


## (5 pts)
 Why does applying a positive voltage to the gate of a CMOS transistor cause the
transistor to conduct between source and drain?

The objective of the problem is to show your understanding of how a CMOS works.

The gate of a CMOS transistor is in between the source and drain but raised up. Applying a positive voltage to the gate of a CMOS transistor will attract electrons to fill the cavity created by the source, drain, and gate, therefore creating a path of electrons for the current to travel on. 

## (5 pts)
Which Boolean operation, AND, OR or NOT, is appropriate for each of the following:
- a. Detecting motion in any motion sensor surrounding a house (each motion sensor outputs 1 when motion is detected).
- b. Detecting that three buttons are being pressed simultaneously (each button outputs 1 when a button is being pressed).
- c. Detecting the absence of light from a light sensor (the light sensor outputs 1
when light is sensed).

The objective of the problem is to demonstrate your ability to implement Boolean operations in real world situations. 
- a.	OR
- b.	AND
- c.	NOT

## (5 pts)
Evaluate the Boolean equation F = (a AND b) OR c OR d for the given values of
variables a, b, c, and d:
- a. a=1, b=1, c=1, d=0
- b. a=0, b=1, c=1, d=0
- c. a=1, b=1, c=0, d=0
- d. a=1, b=0, c=1, d=1

The objective of the problem is to demonstrate your knowledge of Boolean operators. 

![HW2-6](https://github.com/ee260-spring-2019/week-03-jessicaj15/blob/master/docs/assg/HW1.PNG)

## (5 pts)
Convert each of the following equations directly to gate-level circuits:
- a. F = ab’ + bc + c’
- b. F = ab + b’c’d’
- c. F = ((a + b’) * (c’ + d)) + (c + d + e’)

* A. ![HW2_7a](https://github.com/ee260-spring-2019/week-03-jessicaj15/blob/master/docs/assg/Hw2a.PNG)
* B. ![HW2_7b](https://github.com/ee260-spring-2019/week-03-jessicaj15/blob/master/docs/assg/Hw2b.PNG)
* C. ![HW2_7c](https://github.com/ee260-spring-2019/week-03-jessicaj15/blob/master/docs/assg/Hw2c.PNG)


## (5 pts)
We want to concisely describe the following situation using a Boolean equation. We
want to fire a football coach (by setting F=1) if he is mean (represented by M=1). If
he is not mean, but has a losing season (represented by the Boolean variable L=1),
we want to fire him anyways. Write an equation that translates the situation directly
to a Boolean equation for F, without any simplification.

The objective of the problem is to show your ability to translate a real-world scenario into a Boolean expression.  

We are trying to figure out of the coach is being fired (end result) so the entire expression can be represented as F. He will be fired, or F = 1, if: He is mean (M = 1), or in terms of F, F = M. 
He will also be fired if he is not mean (M = 0; M’ = 1) but has a losing season (L = 1). The word ‘but’ indicates that both situations must be true, so this can be represented by an AND operation. In terms of F this situation can be written as: F = (M’) *(L)
Since either situation is possible, we can combine the two situations with an OR operation, so the final expression will be: 
F = M + M’L
