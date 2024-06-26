# Kelvin-Wake-Problem
In this note, we study an interesting problem that comes on usual basis in the domain of fluid dynamics which was historically first studied by Lord Kelvin. This problem is therefore referred as Kelvin-Wake Problem in which we are interested in calculating the following integral:
```math
z\left(\phi,\rho\right)=\int_{-\pi/2}^{\pi/2}\cos\left[\rho\frac{\cos(\theta-\phi)}{\cos^2\theta}\right]d\theta.
```
The parameters present in the above mathematical quantity are defined as follows:
```math
\phi={\tan}^{-1}\dfrac{y}{x}\\
\rho=r\frac{g}{u^2}.
```
Upon the integration of the integrand, we have following figure:
![The Kelvin-Wake Problem](https://github.com/himanshuvnm/Kelvin-Wake-Problem/blob/main/kelvin-wake.png "The Kelvin-Wake Problem")
## Parts of the V-shape of the Kelvin-Wake-Problem
Just, for the simplicity to handle the notation, we let $z\left(\phi,\rho\right)=\mathcal{I}_c(\phi,\rho)$.  We further configured individual parts of the V-shaped present in the above figure of the Kelvin-Wake problem. This leads to have following two integrals summation given as:
```math
\mathcal{I}_c(\phi,\rho)=\int_{-\pi/2}^{\pi/2}\cos\left(\rho\frac{\cos(\theta-\phi)}{\cos^2\theta}\right)d\theta=\underbrace{\int_{-\pi/2}^{0}\cos\left(\rho\frac{\cos(\theta-\phi)}{\cos^2\theta}\right)d\theta}_\text{Part -1}+\underbrace{\int_{0}^{\pi/2}\cos\left(\rho\frac{\cos(\theta-\phi)}{\cos^2\theta}\right)d\theta}_{\text{Part-2}}.
```
A further integral analysis can help us to realize that Part 1 integral is $\int_{-\pi/2}^{0}\cos\left(\rho\frac{\cos(\theta-\phi)}{\cos^2\theta}\right)d\theta≡\int_0^{\pi/2}\cos\left(\rho\frac{\cos(\theta+\phi)}{\cos^2\theta}\right)d\theta.$ Then, the usual routine yields follwoing two figures:

![The Kelvin-Wake Problem: Lower part of V-shape](https://github.com/himanshuvnm/Kelvin-Wake-Problem/blob/main/kelvin-wake%20lower-part.png "The Kelvin-Wake Problem")
![The Kelvin-Wake Problem: Lower part of V-shape](https://github.com/himanshuvnm/Kelvin-Wake-Problem/blob/main/kelvin-wake%20upper-part.png "The Kelvin-Wake Problem")
### Further analysis on the integral
It is interesting to know that the $\mathcal{I}_C\left(\phi,\rho\right)=\mathcal{I}_S\left(\phi,\rho\right)$ where 
```math
\mathcal{I}_S\left(\phi,\rho\right)=\int_0^{\pi/2}\left\{\cos\left(\rho\frac{\sin(\theta+\phi)}{\sin^2\theta}\right)+\cos\left(\rho\frac{\sin(\theta-\phi)}{\sin^2\theta}\right)\right\}d\theta.
```
For the proof, refer the jupyter file. The study in this was inspired and motivated from https://scipython.com/blog/the-kelvin-wake-pattern/.
