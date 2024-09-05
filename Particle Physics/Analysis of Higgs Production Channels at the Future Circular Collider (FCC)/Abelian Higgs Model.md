The central question of electroweak in physics before the discovery of Higgs boson was

> Why are the $W$ and $Z$ boson masses non-zero?

The measured values were, $M_W = 80 \text{GeV}$ and $M_Z = 91\text{GeV}$ far from numbers that one could consider as small effects. 

Is this a problem? Well, yes. consider the following $U(1)$ gauge theory, with a single gauge field, the photon. 
$$
L = -\frac14 F_{\mu\nu}F^{\mu\nu}
$$
where
$$
F_{\mu\nu} = \partial_\nu A_\mu - \partial_\mu A_\nu
$$
The statement of local $U(1)$ gauge invariance means that the lagrangian would be invariant under the transformation of:

$$
A_\mu(x) \rightarrow A_\mu(x) - \partial_\mu \eta(x)
$$
for any $\eta$.  Let's check this invariation:
$$
\begin{align}
F_{\mu\nu} &= \partial_\nu A_\mu - \partial_\mu A_\nu\\
&=\partial_\nu \left(
A_\mu - \partial_\mu\eta
\right) - \partial_\mu\left(
A_\nu-\partial_\nu\eta
\right)\\
&= \partial_\nu A_\mu - \partial_\mu A_\nu -\cancel{\partial_\nu\partial_\mu\eta} + \cancel{\partial_\mu\partial_\nu\eta} \\
& = F_{\mu\nu}
\end{align}
$$
Now the lagrangian is invariance as well (notice that the terms inside of it would not change therefore, it cannot be affected by the change).

Now let's assume that we enter a  term of mass:
$$
L = -\frac14 F_{\mu\nu}F^{\mu\nu} +\frac12 m^2 A_\mu A^\mu
$$
Obviously in this case the second term would not be invariant under the assumed transformation. Therefore it is gauge invariance that requires the photon to be massless.

We now extend the model by adding a single complex scalar field. 
$$
\phi \equiv \frac1{\sqrt2}\left(
\phi_1 + i \phi_2
\right)
$$
Now the lagrangian would take the form:
$$
L = -\frac14 F_{\mu\nu}F^{\mu\nu}+ \left|D_\mu \phi\right|^2 - V(\phi)
$$
Where 
$$
D_\mu = \partial_\mu - ieA_\mu
$$
and 
$$
V(\phi) = \mu^2|\phi|^2+\lambda(|\phi|^2)^2
$$
$V(\phi)$ is the most general renormalizable potential allowed by the $U(1)$ invariance. This lagrangian is invariant under $U(1)$ rotations, $\phi \rightarrow e^{i\theta}\phi$, and under gauge local transformations. namely:
$$
\begin{align}
A_\mu &\rightarrow A_\mu + \partial_\mu \eta\\ 
\phi &\rightarrow e^{-ie\eta}\phi
\end{align}
$$
Here we have two possibilities. If $\mu^2 > 0$  then the potential has the shape that preserves the symmetry of the Lagrangian. The state of the lowest energy is that with $\phi = 0$, the vacuum state.

The theory is simply quantum electrodynamic with massless photon and a charged scalar field $\phi$ with mass $\mu$.

The alternative scenario is more interesting. That is to take $\mu^2 < 0$, then we are able to transform the potential into:

$$
V(\phi) = -|\mu|^2|\phi|^2 + \lambda(|\phi|^2)^2
$$
which has the shape of a mexican hat (something like the image below). In this case the minimum energy state is not at $\phi=0$ but at the point where:
$$
\left\langle\phi\right\rangle = \sqrt{-\frac{\mu^2}{2\lambda}}
$$

![[Pasted image 20240830210630.png]]

This is called vacuum expectation value (VEV) of $\phi$. Note that the direction in which the vacuum is chosen is arbitraty. But it is conventional to choose the direction in which it lies on the real axis.

It is convenient to write $\phi$ as below:
$$
\phi \equiv \frac{1}{\sqrt 2}e^{i\frac\chi v}\left(v + H\right)
$$
Here $\chi$ and $H$ are real fields without any vacuum expectation value. Now we put the newly defined $\phi$ back into the lagrangian and the results are interactions in terms of fields without vacuum expectation values. 
$$
\begin{align}
L &= -\frac14 F_{\mu\nu}F^{\mu\nu} - evA_\mu \partial^\mu \chi \\
&+ \frac{e^2v^2}{2}A_\mu A^\mu + \frac12 \left(
	\partial_\mu H\partial^\mu H + 2\mu^2 H^2\right) \\ &+\frac12 \partial_\mu\chi\partial^\mu \chi
	\\ &+ (H \text{ and } \chi \text{ interactions.})
\end{align}
$$
The second term in the lagrangian is confusing. Therefore, we would use our ability to transform $A_\mu \rightarrow A_\mu -\frac1{ev}\partial_\mu \chi$. After making this gauge transformation the $\chi$ field disappears from the theory and we say that it has been "_eaten_" to give the photon the mass. The $\chi$ field is often called as the Goldenstone boson. The field $H$ is called the Higgs boson. 

The Higgs Mechanism can be summarized by saying that the spontaneous breaking of a gauge theory by a non-zero vacuum expectation value, results in the disappearance of a Goldenstone Boson and its transformation into a longitudinal component of a massvie gauge boson.

It is instructive to count the degrees of freedom. BEfore the spontaneous symmetry breaking there was a massless photon (2 degrees) and a complex scalar field (2 degrees) for a total of 4 degrees of freedom. After the spontaneous symmetry breaking there is a massive photon (3degrees) and a real scalar, $H$, (1 degree) for the same total degrees of freedom. 

At this point let us make an aside about the gauge dependance of these results. The gauge choice above with the transformation $A_\mu \rightarrow A_\mu -\frac{1}{ev}\partial_\mu\chi$ is called the unitary gauge. This gauge has the advantage that the particle spectrum is obvious and there is no $\chi$ field. The unitary gauge however has the disadvantage that the vector proapagator, $\Delta_{\mu\nu}(k)$ has bad high energy behaviour,

$$
\Delta_{\mu\nu}(k) = -\frac{i}{k^2 - M_A^2}\left(g_{\mu\nu} - \frac{k^\mu k^\nu}{M_A^2} \right)
$$

In the unitary gauge scattering cross sections have contributions which grow with powers of $k^2$ which cannot be removed by the conventional mass, coupling constant, and wavefunction renormalizations. More convenient gauges are the so-called $R_\xi$ gauges which are obtained by adding the gauge fixing term to the Lagrangian.

$$
L_{GF} = -\frac1{2\xi}\left(\partial_\mu A^\mu + \xi ev \chi\right)^2
$$
Different choices for $\xi$ correspond to different gauges. In the limit $\xi\rightarrow \infty$  the unitary gauge is recovered. Note that the cross term in this rqeuation cancels the mixed term of the lagrangian. The gauge boson propagator in $R_\xi$ is given by:

$$
\Delta_{\mu\nu}(k) = -\frac{i}{k^2-M^2_A}\left(g_{\mu\nu} -\frac{(1-\xi) k_\mu k_\nu}{k^2 -\xi M^2_A}\right)
$$

In the $R_\xi$ gauges the $\chi$ field is the part of the spectrum and has mass $M^2_\chi = \xi M^2_A$. Feynman gauge corresponde to the choice $\xi =1$ and massless Goldstone bosons with no coupling to the physical Higgs boson. The Landau gauge is often the most convenient for calculations involving the Higgs boson since there is no coupling to the unphysical $\chi$ field.
