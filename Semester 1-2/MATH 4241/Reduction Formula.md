
## Example 1

For $x^n e^x$  

$$u = x^n ~\& ~ v = e^x$$

$$
\begin{align*}
Let, ~ I_n &= \int x^n e^x dx \\
&= x^n e^x - \int (nx^{n-1}\int e^x dx)dx\\
&= x^n e^x - \int n x^{n-1} e^xdx\\
&= x^n e^x - n \int x^{n-1} e^xdx\\
&= x^n e^x - n ~I_{n-1}\\
\end{align*}
$$

Now, for $\int x^4e^x ~dx$

$$
\begin{align*}\therefore \int x^4 e^x \, dx &= x^4 e^x - 4I_3 \\&= x^4 e^x - 4[x^3 e^x - 3I_2] \\&= x^4 e^x - 4x^3 e^x + 12I_2 \\&= x^4 e^x - 4x^3 e^x + 12[x^2 e^x - 2I_1] \\&= x^4 e^x - 4x^3 e^x + 12x^2 e^x - 24I_1 \\&= x^4 e^x - 4x^3 e^x + 12x^2 e^x - 24[x e^x - 1I_0] \\&= x^4 e^x - 4x^3 e^x + 12x^2 e^x - 24xe^x + 24I_0 \\&= x^4 e^x - 4x^3 e^x + 12x^2 e^x - 24xe^x + 24e^x + C\end{align*}
$$

### Reduction Formula $sin ^nx$

$$
\begin{align*}
I_n &= \sin^{n-1}x(-\cos x) - \int (n-1)\sin^{n-2}x \cos x(-\cos x)dx \\
&= -\sin^{n-1}x \cos x + (n-1)\int \sin^{n-2}x \cos^2 x\,dx \\
&= -\sin^{n-1}x \cos x + (n-1)\int \sin^{n-2}x(1-\sin^2 x)\,dx \\
&= -\sin^{n-1}x \cos x + (n-1)\int \sin^{n-2}x\,dx - (n-1)\int \sin^n x\,dx \\
I_n&= -\sin^{n-1}x \cos x + (n-1)I_{n-2} - (n-1)I_n
\end{align*}
\\~\\
\therefore I_n = \frac{-\sin^{n-1}x \cos x}{n} + \frac{n-1}{n}I_{n-2} \quad \\ \text{is the required reduction formula for } \int \sin^n x \, dx 
$$

### Reduction Formula $cos^nx$
$$\begin{align}
  \int \cos^n x  & = \int \cos^{n-1}x \times \cos x dx \\
 I_{n}& = \cos ^{n-1}x \int \cos x - \int \left( {(n-1)\cos^{n-2}x \ \sin x \int{\cos x}\ }  \right)\ dx  \\
 & = \cos ^ {n-1 } x \ \sin x - (n-1)\int{\cos^{n-2} x \sin^2 {x}}\ dx  \\
 & = \cos^{n-1} x \ \sin x - (n-1) \int {\cos ^ {n-2}- \cos^n x } \ dx   \\
	 & = \cos^{n-1} x \ \sin x - (n-1) \int {\cos ^{n-1} x } \ dx - (n-1) \ I_{x} \ dx  \\
 I_{n} + (n-1 ) I_{n}  & = \cos ^{n-1} x \sin x - (n-1 )\int \cos ^{n-1 } x \ dx \\
I_{n} & = \frac{\cos ^{n-1}\sin x }{n} + \frac{n-1}{n}I_{n-2} \\
\end{align}$$


