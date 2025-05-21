

using $\int uv \, dx = u \int v \, dx - \int \left( u' \int v \, dx \right) dx$
### Reduction Formula for $\int x^n e^x dx$
  
For $x^n e^x$  

$$u = x^n ~\& ~ v = e^x$$
$$\begin{align*}

\text{Let, } I_n &= \int x^n e^x dx \\


&= x^n e^x - \int (nx^{n-1}\int e^x dx)dx\\

&= x^n e^x - \int n x^{n-1} e^xdx\\

&= x^n e^x - n \int x^{n-1} e^xdx\\

&= x^n e^x - n ~I_{n-1}

\end{align*}$$


### $\int x^4 e^x \, dx$

$$\begin{align*}\therefore \int x^4 e^x \, dx &= x^4 e^x - 4I_3 \\&= x^4 e^x - 4[x^3 e^x - 3I_2] \\&= x^4 e^x - 4x^3 e^x + 12I_2 \\&= x^4 e^x - 4x^3 e^x + 12[x^2 e^x - 2I_1] \\&= x^4 e^x - 4x^3 e^x + 12x^2 e^x - 24I_1 \\&= x^4 e^x - 4x^3 e^x + 12x^2 e^x - 24[x e^x - 1I_0] \\&= x^4 e^x - 4x^3 e^x + 12x^2 e^x - 24xe^x + 24I_0 \\&= x^4 e^x - 4x^3 e^x + 12x^2 e^x - 24xe^x + 24e^x + C\end{align*}$$

  
### Reduction Formula for $sin ^nx​$

$$\begin{align*}

I_n &= \sin^{n-1}x(-\cos x) - \int (n-1)\sin^{n-2}x \cos x(-\cos x)dx \\

&= -\sin^{n-1}x \cos x + (n-1)\int \sin^{n-2}x \cos^2 x\,dx \\

&= -\sin^{n-1}x \cos x + (n-1)\int \sin^{n-2}x(1-\sin^2 x)\,dx \\

&= -\sin^{n-1}x \cos x + (n-1)\int \sin^{n-2}x\,dx - (n-1)\int \sin^n x\,dx \\

&= -\sin^{n-1}x \cos x + (n-1)I_{n-2} - (n-1)I_n

\end{align*}$$


$$ \therefore I_n = \frac{-\sin^{n-1}x \cos x}{n} + \frac{n-1}{n}I_{n-2} \quad \text{is the required reduction formula for } \int \sin^n x \, dx $$
### Reduction Formula for $\int \cos^n x \, dx$

### Reduction Formula for $\int \sec^n x \, dx$



