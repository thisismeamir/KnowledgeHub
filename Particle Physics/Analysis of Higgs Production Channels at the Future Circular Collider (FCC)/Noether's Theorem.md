Symmetry is an age-old idea that originated in geometry. Despite that symmetry can also be expanded to other fields. In physics, symmetry means that a given law or property remains unchanged under certain transofmrations, such as spatial and time transformations. 

This property implies that we cannot physically differentiate between two distinct configurations of the dynamical variables that describe a syste. Meaning that the action remains invariant. 

Over a century ago, physicists realized that nearly all natural phenomena can be explained by assuming that nature seeks to optimize a certain function, known as the action, denoted by $S$. 

Rather than applying forces on masses to anticipate the progression of an event , which is determined by an initial condition, we can begin with the boundary conditions that describe how the event starts and concludes the account for what happens in between by assuming that nature minimizes the action.

In 1918, Emmy Noether discovered the relationship between the symmetries of action and conserved quantities.

The action is defined as the integration of the Lagrangian density with respect to spatial and temporal coordinates as:

$$
S = \int d^4 x L
$$
The principle of least action states that the path taken by the system between two points in space time is the one that makes the action stationary.

$$ 
\delta S = \delta \int d^4 xL(\phi_a(x), \partial_\mu\phi_a(x))
$$
From this we can derive the familiar Euler-Lagrange equation:
$$
\frac{\partial L}{\partial \phi_a} - \partial_\mu\frac{\partial L}{\partial(\partial_\mu\phi_a)} = 0
$$
and the momentum field is defined as:
$$
\pi_a(x) = \frac{\partial L}{\partial(\partial_0 \phi_a)}
$$
and to quantize the fields, we introduce the following commutation relations:
$$
[\phi_a(x,t), \phi_b(y,t)] = [\pi_a(x,t), \pi_b(y,t)] = 0
$$
and 
$$
[\phi_a(x,t), \pi_b(y,t)] = i\delta_{ab}\delta^3(x-y)
$$
The commutation relations between field operators give rise to fluctuations. There fluctuations represent the ingerent variabilityor uncertainty associated with the field's value at a given point in space and time.

These fluctuations give rise to the creation and annihilation of particles, and they affect the brhavior of the field and its interactions. 

If the transformation $\phi_a \rightarrow \phi_a +\alpha\Delta\phi_a$ is symmetric, wherein $\alpha$ represents an infinitesimal parameter and $\Delta\phi_a$ denotes a deformation in the field configuration, it follows that the Lagrangian must remain invariant under this transformation.

$$ L = L + \alpha\partial_\mu J^\mu $$
for some $J^\mu$. The variation of the Lagrangian density resulting from the variation of the firld is expressed as follows:

$$
\alpha\Delta L  = \frac{\partial L}{\partial \phi_a} + \left(\frac{\partial L}{\partial(\partial_\mu\phi_a)}\right)\partial_\mu (\alpha\Delta\phi_a)
$$
After rearranging terms we get:
$$
\alpha\Delta L = \alpha\left[\frac{\partial L}{\partial \phi_a} - \partial_\mu \left(\frac{\partial L}{\partial(\partial_\mu \phi_a)}\right)\right]\Delta\phi_a +\alpha\partial_\mu\left(\frac{\partial L }{\partial(\partial_\mu\phi_a)}\Delta\phi_a\right)
$$
Since the bracket term is the euler lagrange equation it would vanish. And we're left with:
$$
\alpha\Delta L = \alpha\partial_\mu\left(\frac{\partial L}{\partial(\partial_\mu \phi_a)}\Delta\phi_a\right)
$$
Setting these equal to $\alpha\partial_\mu J^\mu$ we get:
$$
\partial_\mu j^\mu = 0 \ \text{ for } \ j^\mu = \frac{\partial L}{\partial(\partial_\mu \phi_a)} \Delta\phi_a - J^\mu
$$
then the current $j^\mu$ is conserved for continuous symmetries.

this equation shows that if we integrate over all space we get a zero: and as spatial parameters vanish at infinitie we obtain the Gauss' theorem:
$$
\begin{align}
\int d^3x\left(\frac{\partial}{\partial t}j^0 + \vec \nabla\cdot \vec j\right)&=0\\
Q(t) &= \int d^3 x j^0 \\
\frac{dQ(t)}{dt} &= \frac{d}{dt}\int d^3 x j^0
\end{align}
$$
$$
\boxed{
\frac{dQ(t)}{dt} = 0
}
$$
The fact that $\partial_\mu j^\mu = 0$ is known as the conservation law and it can be associated with a conserved quantity, which is given by the integral over space of the time component of the current $j^0$:
$$
Q(t) \int d^3 x j^0(x,t)
$$
If $\partial_\mu j^\mu = 0$, then $Q(t)$ is conserved. This is the core of Noether's theorem, which claims that a corresponding conserved quantity exists for any continuous symmetry of the Lagrangian.

[[Gauge Invariance]]