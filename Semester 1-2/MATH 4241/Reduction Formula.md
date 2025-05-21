  

using $\int uv \, dx = u \int v \, dx - \int \left( u' \int v \, dx \right) dx$
# Reduction Formula for $\int x^n e^x dx$

  

$$\begin{align*}

\text{Let, } I_n &= \int x^n e^x dx \\

&= x^n e^x - \int (nx^{n-1}\int e^x dx)dx\\

&= x^n e^x - \int n x^{n-1} e^xdx\\

&= x^n e^x - n \int x^{n-1} e^xdx\\

&= x^n e^x - n ~I_{n-1}

\end{align*}$$

  

### $\int x^4 e^x \, dx$

$$\begin{align*}\therefore \int x^4 e^x \, dx &= x^4 e^x - 4I_3 \\&= x^4 e^x - 4[x^3 e^x - 3I_2] \\&= x^4 e^x - 4x^3 e^x + 12I_2 \\&= x^4 e^x - 4x^3 e^x + 12[x^2 e^x - 2I_1] \\&= x^4 e^x - 4x^3 e^x + 12x^2 e^x - 24I_1 \\&= x^4 e^x - 4x^3 e^x + 12x^2 e^x - 24[x e^x - 1I_0] \\&= x^4 e^x - 4x^3 e^x + 12x^2 e^x - 24xe^x + 24I_0 \\&= x^4 e^x - 4x^3 e^x + 12x^2 e^x - 24xe^x + 24e^x + C\end{align*}$$

  
  
  
  

# Reduction Formula for $sin ^nx​$

  

$$\begin{align*}

I_n &= \sin^{n-1}x(-\cos x) - \int (n-1)\sin^{n-2}x \cos x(-\cos x)dx \\

&= -\sin^{n-1}x \cos x + (n-1)\int \sin^{n-2}x \cos^2 x\,dx \\

&= -\sin^{n-1}x \cos x + (n-1)\int \sin^{n-2}x(1-\sin^2 x)\,dx \\

&= -\sin^{n-1}x \cos x + (n-1)\int \sin^{n-2}x\,dx - (n-1)\int \sin^n x\,dx \\

&= -\sin^{n-1}x \cos x + (n-1)I_{n-2} - (n-1)I_n

\end{align*}$$

  

$$ \therefore I_n = \frac{-\sin^{n-1}x \cos x}{n} + \frac{n-1}{n}I_{n-2} \quad \text{is the required reduction formula for } \int \sin^n x \, dx $$

  
  
  
  
  

# Reduction Formula for $\int \cos^n x \, dx$.

Let, $I_n = \int \cos^n x \, dx$.

We apply integration by parts. Let $u = \cos^{n-1}x$ and $dv = \cos x \, dx$.

Then $du = (n-1)\cos^{n-2}x (-\sin x) \, dx$ and $v = \sin x$.

  

$$

\begin{aligned} % Use aligned inside $$ for multiple lines, or align* if the whole block is just this.

I_n &= \cos^{n-1}x(\sin x) - \int (\sin x) [-(n-1)\cos^{n-2}x \sin x] \, dx \\

&= \sin x \cos^{n-1}x + (n-1)\int \cos^{n-2}x \sin^2 x \, dx \\

&= \sin x \cos^{n-1}x + (n-1)\int \cos^{n-2}x (1-\cos^2 x) \, dx \\

&= \sin x \cos^{n-1}x + (n-1)\int \cos^{n-2}x \, dx - (n-1)\int \cos^n x \, dx \\

&= \sin x \cos^{n-1}x + (n-1)I_{n-2} - (n-1)I_n

\end{aligned}

$$

Collecting terms involving $I_n$:

$$

\begin{aligned}

I_n + (n-1)I_n &= \sin x \cos^{n-1}x + (n-1)I_{n-2} \\

n I_n &= \sin x \cos^{n-1}x + (n-1)I_{n-2}

\end{aligned}

$$

$$ \therefore I_n = \frac{\sin x \cos^{n-1}x}{n} + \frac{n-1}{n}I_{n-2} $$

This is the required reduction formula for $\int \cos^n x \, dx$.

  
  
  
  

## Reduction Formula for $\int \sec^n x \, dx$

Let $I_n = \int \sec^n x \, dx$.

We strategically break down $\sec^n x$ as $\sec^{n-2}x \cdot \sec^2 x$.

  
Let:

$u = \sec^{n-2}x$

$v = \sec^2 x$

Now, we find $u'$ and $\int v \, dx$:

1.  Find $u'$ (derivative of $u$)

    $$u' = \frac{d}{dx}(\sec^{n-2}x) = (n-2)\sec^{n-3}x \cdot (\sec x \tan x) = (n-2)\sec^{n-2}x \tan x$$

  
2. Find $\int v \, dx$ (integral of $v$):

    $$\int v \, dx = \int \sec^2 x \, dx = \tan x$$

  

Substitute these into the formula $\int uv \, dx = u \int v \, dx - \int \left( u' \int v \, dx \right) dx$:

$$

\begin{aligned}

I_n &= \sec^{n-2}x (\tan x) - \int \left( (n-2)\sec^{n-2}x \tan x \cdot \tan x \right) dx \\

&= \sec^{n-2}x \tan x - (n-2)\int \sec^{n-2}x \tan^2 x \, dx

\end{aligned}

$$

Use the trigonometric identity $\tan^2 x = \sec^2 x - 1$:

$$

\begin{aligned}

I_n &= \sec^{n-2}x \tan x - (n-2)\int \sec^{n-2}x (\sec^2 x - 1) \, dx \\

&= \sec^{n-2}x \tan x - (n-2)\int (\sec^n x - \sec^{n-2}x) \, dx \\

&= \sec^{n-2}x \tan x - (n-2)\left( \int \sec^n x \, dx - \int \sec^{n-2}x \, dx \right) \\

&= \sec^{n-2}x \tan x - (n-2)I_n + (n-2)I_{n-2}

\end{aligned}

$$

Now, collect terms involving $I_n$ on the left side:

$$

\begin{aligned}

I_n + (n-2)I_n &= \sec^{n-2}x \tan x + (n-2)I_{n-2} \\

I_n (1 + n - 2) &= \sec^{n-2}x \tan x + (n-2)I_{n-2} \\

I_n (n - 1) &= \sec^{n-2}x \tan x + (n-2)I_{n-2}

\end{aligned}

$$

Finally, divide by $(n-1)$ (assuming $n \ne 1$):

$$ \therefore I_n = \frac{\sec^{n-2}x \tan x}{n-1} + \frac{n-2}{n-1}I_{n-2} $$

This is the required reduction formula for $\int \sec^n x \, dx$.
