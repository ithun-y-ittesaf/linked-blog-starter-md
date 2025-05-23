

![[Lecture 4 _Successive Reduction.pdf]]



using $\int uv \, dx = u \int v \, dx - \int \left( u' \int v \, dx \right) dx$
### Reduction Formula for $\int x^n e^x dx$
  

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
$$\begin{align*}
I_n &= \int \cos^n x \, dx 
     = \int \cos^{n-1} x \,\cos x \, dx \\[6pt]
    &= \int \cos^{n-1} x \, d(\sin x) \\[4pt]
    &= \cos^{n-1} x \,\sin x
       - \int \sin x \,d\bigl(\cos^{n-1} x\bigr) \\[4pt]
    &= \cos^{n-1} x \,\sin x
       + (n-1)\int \sin^2 x \,\cos^{n-2} x \, dx \\[4pt]
    &= \cos^{n-1} x \,\sin x
       + (n-1)\int \bigl(1 - \cos^2 x\bigr)\cos^{n-2} x \, dx \\[4pt]
    &= \cos^{n-1} x \,\sin x
       + (n-1)\,I_{n-2}
       - (n-1)\,I_n \\[6pt]
n\,I_n &= \cos^{n-1} x \,\sin x
         + (n-1)\,I_{n-2} \\[6pt]
&\boxed{%
I_n = \frac{\cos^{n-1} x \,\sin x}{n}
      + \frac{n-1}{n}\,I_{n-2}
      + C
}
\end{align*}$$
### Reduction Formula for $\int \sec^n x \, dx$

$$\begin{align*}
I_n &= \int \sec^n x \, dx 
     = \int \sec^{n-2} x \,\sec^2 x \, dx \\[6pt]
    &= \underbrace{\sec^{n-2} x \,\tan x}_{u\cdot v}
       - (n-2)\int \sec^{n-2} x \,\tan^2 x \, dx \\[6pt]
    &= \sec^{n-2} x \,\tan x 
       - (n-2)\int \sec^n x \, dx 
       + (n-2)\int \sec^{n-2} x \, dx \\[6pt]
(n-1)\,I_n &= \sec^{n-2} x \,\tan x 
             + (n-2)\,I_{n-2} \\[6pt]
&\boxed{%
I_n = \int \sec^n x \, dx
    = \frac{\sec^{n-2} x \,\tan x}{n-1}
      + \frac{n-2}{\,n-1\,}\,I_{n-2}
      + C
}
\end{align*}$$






