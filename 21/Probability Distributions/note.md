## [Normal Distribution](https://en.wikipedia.org/wiki/Normal_distribution)

The normal distribution, also known as the Gaussian distribution, is a continuous probability distribution characterized by its bell-shaped curve. It is defined by two parameters: the mean (μ) and the standard deviation (σ). The probability density function (PDF) of the normal distribution is given by:

![Normal Distribution PDF](https://upload.wikimedia.org/wikipedia/commons/8/8c/Standard_deviation_diagram.svg)

The formula for the PDF is:

$$f(x) = \frac{1}{\sqrt{2\pi\sigma^2}} e^{-\frac{(x - \mu)^2}{2\sigma^2}}$$

Where:
- $f(x)$ is the value of the PDF at point $x$
- $\mu$ is the mean
- $\sigma$ is the standard deviation
- $e$ is the base of the natural logarithm

**Definition:** A random variable $X$ is said to have a normal distribution with
parameters $μ$ (called "mean") and $σ^2$ (called "variance") if its density function
is given by the probability law:

$$f(x) = \frac{1}{\sqrt{2\pi\sigma^2}} e^{-\frac{(x - \mu)^2}{2\sigma^2}}$$

**Remarks.** 
1. A random variable $X$ with mean $\mu$ and variance $\sigma^2$ and
following the normal law - is expressed by $X \sim N(\mu, \sigma^2)$.
2. If $X \sim N(\mu, \sigma^2)$, then $Z = \frac{X - \mu}{\sigma}$ is a standard normal variate with
$E(Z) = 0$ and $Var(Z) = 1$ and we write $Z \sim N(0, 1)$.
3. The p.d.f. of standard normal variate $Z$ is given by
$$\phi(z) = \frac{1}{\sqrt{2\pi}} e^{-\frac{z^2}{2}}, -\infty < z < \infty$$
and the corresponding distribution function, denoted by $\Phi(z)$, is given by
$$\Phi(z) = P(Z \leq z) = \int_{-\infty}^{z} \phi(u) \, du = \frac{1}{\sqrt{2\pi}} \int_{-\infty}^{z} e^{-\frac{u^2}{2}} \, du$$

* Two important results on the distribution function
    1. $\Phi(-z) = 1 - \Phi(z)$ [link](https://share.google/aimode/LLJ5WUS2m2E5B7Yhh)
    2. $P(a \leq X \leq b) = \Phi\left(\frac{b - \mu}{\sigma}\right) - \Phi\left(\frac{a - \mu}{\sigma}\right)$
where $X \sim N(\mu, \sigma ^ 2)$ [link](https://share.google/aimode/llwKwE15tnMBFX0zZ)

4. The graph of $\phi(x)$ is a famous *'bell-shaped'* curve. The top of the bell
is directly above the mean $\mu$. For large values of $\sigma$, the curve tends to flatten out
and for small values of $\sigma$, it has a sharp peak.

### Normal Distribution as a Limiting form of Binomial Distribution.
The normal distribution can be derived as a limiting case of the binomial distribution under certain conditions.
1. the number of trials is indefinitely large. That is, $n \to \infty$ and
2. neither $p$ nor $q$ is very small.

Mathematically, if $X \sim Binomial(n, p)$, then as $n \to \infty$ and $p \to 0$ such that $np = \mu$ is constant, we have:

$$X \sim N(\mu, \sigma^2)$$

This result is a consequence of the Central Limit Theorem, which states that the sum of a large number of independent and identically distributed random variables tends toward a normal distribution, regardless of the original distribution of the variables.
