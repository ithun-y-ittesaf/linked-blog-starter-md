
A digital system is an electronic system that processes stores and communicates information using digital data. 
Digital systems form the backbone of modern technology playing a critical role in communication …..

What Does “Digital” Means?

Digital means  to data or signals that. are represented by discrete values.

Digital Data
Analog date  closely mirror to real-world phenomena, difficult to process, using electronic system, cause its highly susceptible to noise, distortion, and signal degradation

## Gray Code vs Binary

To change number from 3 to 4

In binary we need to change 3 different memory 011 → 100

For gray Code, only one memory change is needed 010 → 110

Always in gray Code, only one memory block needs to be changed to go to next number

### Gray Code and Binary Conversion

<h4>Binary to Gray Code</h4>

![[image 1 1.png]]

<h4> Gray to Binary Code</h4>
![[image.png]]
`
## Excess-3

Obtained from the corresponding **BCD+3**

## Diminished Radix Complement

(r-1)’s complement of N (here, r is Base of N)

$$
r^n-r^{-m} - N
$$

Example:

- 9’s complement of $(25.639)_{10}= 10^2 - 10^{-3} - (25.639)_{10} = (74.360)_{10}$
- 1’s complement of $(1011.101)_2 = 2^4 - 2^{-3}-1011.101 = (0100.010)_2$

## Radix Complement

r’s Complement of N (here, r is Base of N)

$$
r^n-N
$$

Example:

- 10’s complement of $(25.639)_{10}= 10^2  - (25.639)_{10} = (74.361)_{10}$
- 2’s complement of $(1011.101)_2 = 2^4-1011.101 = (0100.011)_2$

$$
(r-1)'s + 1_{LSB} = r's
$$

## BCD Arithmetic

$$
786 -> 0111~1000~0110\\
162 -> 0001~0110~0010
$$

---

$$
8(14)8-> 1000~1110~1000
\\948->1001~0100~1000
$$

We add 6 (16-10) to the Binary value of 14 to convert it to 1 4 in BCD

$$
~~~1110\\
+0110
$$

---

$$
1~0100\\
1 ~~~~4
$$