Symmetry under group $U(1)$ in quantum electrodynamics (QED), refers to the fact that the equations describing the behavior of particles remain unchanged if the electron field and the gauge field are multiplied by a phase $e^{i\theta}$. 

The $U(1)$ is represented by a circle, where each point on the circle corresponds to an element of the group. Multiplying two elements of this group involves adding their corresponding angles, which corresponds to rotating around the circle. 

The phase of a wavefunction can be altered by multiplying it by a complex number. This corresponds to a change in the wavefunction's general "form" or "look" but not any of its actual characteristics, such as its probability distribution.

In the framework of QED's $U(1)$ symmetry, multiplying the electron and gauge fields by complex numbers of unit magnitude alters their overall phase but has no effect on any of their physical characteristics or the theory's predictions.

Under local transformations, the Dirac Lagrangian undergoes a specific transformation that can be expressed mathematically as:
$$
\begin{align}
L\rightarrow L' &= \bar\psi'(x)(i\gamma^\mu\partial_\mu - m)\psi'(x)\\
&= e^{i\theta(x)}\bar\psi(x)(i\gamma^\mu\partial_\mu - m)e^{i\theta(x)}\psi(x)\\
&=\bar\psi(x)(i\gamma^\mu\partial_\mu - m)\psi(x)+\bar\psi(x) \gamma^\mu\psi(x)\partial_\mu \theta(x)\\
&= \boxed{L + j^\mu(x)\partial_\mu\theta(x)}
\end{align}
$$

where $j^\mu = \bar\psi(x)\gamma^\mu\psi(x)$ is the vector current carried by the fermion. Thus, the Lagrangian is not invariant under local transformation unless $\partial_\mu\theta(x) = 0$, which means that $\theta(x)$ is independent of $x$. The additional gradient-of-phase term spoils local phase invariance. Local phase invariance may be achieved, however, of the equations of motion and the observables involving derivatives are midfied by the introduction of electromagnetic field as:

$$
\partial_\mu\rightarrow D_\mu \equiv \partial_\mu - iqA_\mu(x)
$$
Thus, if we define the Lagrangian by replacing $\partial_\mu$ by $D_\mu$:
$$
\begin{align}
L(\psi,\bar\psi, A_\mu) &= \bar\psi(i\gamma^\mu D_\mu -m)\psi\\
&= \bar\psi(i\gamma^\mu\partial_\mu - m)\psi + q\bar\psi\gamma_\mu\psi A_\mu
\end{align}
$$
This way $L$ becomes invariant under the transformation if at the same time we make the replacement:
$$
A_\mu\rightarrow A_\mu' = A_\mu \frac1q \partial_\mu\theta(x)
$$
which precisely cancels the unwanted term. Then, electromagnetic dynamics is made invariant by introducing a spin 1 vector (gauge)  boson field $A_\mu$ called the photon through the covariant derivative, which is called "minimal coupling". It is very important to know that in the gauge invariant theories, the interaction between gauge bosons and particles is uniquely determined only through the minimal coupling. The Lagrangian, which is invariant under local $U(1)$ gauge transformation, is therefore given by 
$$
L =\bar\psi(i\gamma^\mu D_\mu - m)\psi
$$
but this is not the complete Lagrangian of electrodynamics. We should count for the propagator (photon) mass and a kinetic energy term for the vector field to describe the propagation of free photons.

If we take into account the mass term we have:
$$
L_\gamma = \frac{m^2}{2}A_\mu A^\mu
$$
which violates the local gauge invariance. Therefore, we conclude that photon has mass of  zero.
In the absence of sources an appropriate Lagrangian for the free electromagnetic field is:

$$
L_{\text{QED}} = \bar\psi(x)(i\gamma^\mu D_\mu - m)\psi(x) - \frac14 F_{\mu\nu}F^{\mu\nu} 
$$
where $F_{\mu\nu} F^{\mu\nu}$ is
$$
(\partial_\nu A_\mu - \partial_\mu A_\nu)(\partial^\nu A^\nu - \partial^\nu A^\mu)
$$
