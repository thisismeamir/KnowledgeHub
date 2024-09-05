There are two approaches to addressing symmetry breaking in field thoery. One method involves introducting a term for symmetry breaking alongside the term for symmetry mannually:

$$ L = L_{\text{symmetry}} + L_{\text{breaking}}
$$
This method is effective when the symmetry breaking term is small. In this situation, $L$ retains the exact symmetry of a vanishing $L_{\text{breaking}}$. However it is worth noting that this circumstance is somewhat theoretical, since there is no fundamental principle to dictate the precise structure of the breaking term.

Another method is called *hidden or spontaneous symmetry breaking*, where the Lagrangian remains symmetric under certain group transformations while the physical vacuum is made non-invariant. We denote the free part of the Klein-Gordon Lagrangian density for a complex scalar field as:

$$
L_O = \partial_\mu\phi^\dagger\partial^\mu\phi - m^2\phi^\dagger\phi
$$
To be able to include interactions, the Lagrangian density for the interaction must be invariant under Lorentz transformation, translation, and gauge transformations if the theory has gauge symmetry.

Furthermore, since the free Lagrangian density is invariant under the discrete $Z_2$ symmetry transformation:

$$
\phi(x) \leftrightarrow \phi^\dagger(x)
$$
We would also like to preserve this symmetry in interactions. With these conditions, the simplest interaction Lagrangian density for a complex scalar field has the form:

$$
L_I = -\frac\lambda4 (\phi^\dagger \phi)^2
$$
This term describes the most general renormalizable self-interacting theory for a complex Klein-Gordon field.

The system is equivalent to the one described by the following Lagrangian composed of $2$ real fields $\psi_1, \psi_2$ which are related to $\phi$ and $\phi^\dagger$ as 

$$
\phi =\frac{\psi_1 + i\psi_2}{\sqrt{2}}
$$
and 
$$
\phi^\dagger = \frac{\psi_1 - i\psi_2}{\sqrt{2}}
$$
the Lagrangian is:

$$
L = \frac12\partial_\mu\psi_1\partial^\mu\psi_1 + \frac12\partial_\mu\psi_2\partial^\mu\psi_2 - V(\psi_1^2+\psi_2^2),
$$

Which has $O(2)$ symmetry, meaning that rotating the field values at each point by an angle does not change the overall proerties of the field.