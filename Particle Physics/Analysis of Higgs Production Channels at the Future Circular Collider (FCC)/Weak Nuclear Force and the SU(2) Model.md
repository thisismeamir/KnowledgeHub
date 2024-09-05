After the success of Quantum Electrodynamics (QED), The was to find a mathematical framework that could incorporate gauge symmetries and describe all known particles and their interactions.

In 1950s, Chen Ning Yang and Robert Mills proposed a generalization of gauge theories to include non-Abelian gauge Symmetries. The Mathematical framework for describing interactions mediated by multiple gauge bosons, allowing for the incorporation of strong and weak nuclear forces.

The experimental evidence supporting the existence of strong and weak nuclear forces provided further motivation. Also observations such as $\beta$-decay were hinting to another theory.

Conseider two fermion fields, two spin $\frac12$ fields, $\psi_1$ and $\psi_2$, then the Lagrangian of the system without any interactions is just the sum of two Diract Lagrangians:

$$
\begin{align}
L = \ &L_1 + L_2\\
= \ &\bar\psi_1(x) (i\gamma^\mu\partial_\mu - m_1)\psi_1(x)\\ 
 &+ \bar\psi_2(x) (i\gamma^\mu\partial_\mu - m_2)\psi_2(x)
\end{align}
$$
We can define 

$$
\psi = \begin{pmatrix} \psi_1 \\ \psi_2 \end{pmatrix}
$$
and 

$$
M = \begin{pmatrix}
m_1 & 0 \\ 
0 & m_2
\end{pmatrix}
$$
then the complete Lagrangian is:

$$
L = \bar\psi(i\gamma^\mu\partial_\mu - M)\psi
$$
Now, $L$ can possess a broader global invariance compared to the previous case, as:

$$
\psi\rightarrow \psi' = U\psi
$$
Where $U$ is a unitary matrix. Thus:

$$
\bar\psi \rightarrow \bar\psi' = \bar\psi U^{\dagger}
$$
Therefore, $\bar\psi\psi$ is invariant.As $U$ is unitary, it can be expressed as $U = e^{iH}$, where $H$ is a Hermitian matrix. It is known that one can expand any hermitian matrix in terms of pauli matrices:

$$
H = a_0 I + a_i\tau_1 + a_2\tau_2 + a_3\tau_3 = a_0 I + \vec a\cdot \vec \tau
$$
Thus any unitary matrix can be written as:

$$
U = e^{ia_0}e^{i\vec a\cdot \vec \tau}
$$
Now focusing on the transformation below:

$$
\psi' = e^{i\vec a\cdot \vec \tau}\psi
$$
This is called global (no spatial dependency) $SU(2)$ transformation. Yang and Mills extended this global invariance to a local gauge invariance.

The first step is to make the parameter $a$ dependent on $x$, I will let $a(x) = -\frac12 g\theta(x)$. Here, $g$ is the coupling strength to be determined from experiments. Thus, 

$$
\psi' = e^{-ig\frac\tau2 \theta(x)}\psi
$$
and

$$
\bar\psi' = e^{ig\frac\tau2\theta(x)}\bar\psi
$$

Then the gradient transforms as:

$$
\partial_\mu\psi' = (\partial_\mu U)\psi + U(\partial_\mu\psi)
$$

Therefore, the new Lagrangian is:

$$
\begin{align}
L' &= \bar\psi'(i\gamma^\mu\partial_\mu - M)\psi'\\
&= e^{ig\frac\tau2\theta(x)}\bar\psi(i\gamma^\mu\partial_\mu - M)e^{ig\frac\tau2\theta(x)}\psi\\
&=\bar\psi(i\gamma^\mu\partial_\mu -M )\psi+(\partial_\mu\theta(x))\bar\psi\left(\gamma^\mu g\frac\tau2\right)\psi\\
&= L + (\partial_\mu\theta(x))\bar\psi\left(\gamma^\mu g\frac\tau2\right)\psi
\end{align}
$$
as you can see this Lagrangian is still not invariant under this transformation. To ensure the local gauge invariance of the theory, we first introduce a gauge covariant derivative, 

$$
\partial_\mu \rightarrow D_\mu = \partial_\mu - ig\vec A_\mu
$$
This derviative should satisfy:

$$
(D_\mu\psi)' = D'_\mu \psi' = UD_\mu(\psi)
$$
Therefore, we start by the left hand side:

$$
\begin{align}
D'_\mu\psi' &= (\partial_\mu - ig\vec A_\mu')\psi'\\
&= (\partial_\mu U)\psi+U(\partial_\mu\psi) - ig A'_\mu(U\psi)
\end{align}
$$
and from the left hand side:
$$
\begin{align}
UD_\mu\psi &= U(\partial_\mu -ig\vec A_\mu)\psi\\
&= U(\partial_\mu\psi) - igU(\vec A_\mu\psi)
\end{align}
$$

Putting these two equal to each other we obtain:

$$
\begin{align}
(\partial_\mu U)\psi + U(\partial_\mu\psi) - ig\vec A_\mu' U\psi &= U(\partial_\mu\psi) - igU(\vec A_\mu\psi)\\
ig\vec A_\mu' U\psi &=(\partial_\mu U)\psi + igU(\vec A_\mu\psi)\\
\end{align}
$$
now substituting $I$ before each $\psi$ occurance we get:

$$
\begin{align}
ig\vec A_\mu'(UU^{-1}U\psi) &= (\partial_\mu U)U^{-1}U\psi + igU(\vec A_\mu U^{-1}U\psi)\\
\vec A'_\mu &= U\vec A_\mu U^{-1}+\frac{-i}{g}(\partial_\mu U)U^{-1}
\end{align}
$$

Now let's check out the Field tensor (old one that we knew) via transformation:

$$
F_{\mu\nu}' = \partial_\mu A_\nu' - \partial_\nu A_\mu'
$$
expanding the terms results in
$$
\begin{align}
= &\partial_\mu\left[
UA_\nu U^{-1} - \frac{i}{g}(\partial_{\nu}U)U^{-1}
\right] \\ &- \partial_\nu\left[
UA_\mu U^{-1} - \frac{i}{g}(\partial_{\mu}U)U^{-1}
\right]
\end{align}
$$

expanding the first term we get:
$$
\begin{align}
a: &(\partial_\mu U)A_\nu U^{-1} + U(\partial_\mu A_\nu)U^{-1} + U A_\nu(\partial_\mu U^{-1})\\ &-\frac{i}{g}\left[
(\partial_\mu\partial_\nu U)+\partial_\nu U\partial_\mu U^{-1}
\right]
\end{align}
$$
and the second term
$$
\begin{align}
b: &(\partial_\nu U)A_\mu U^{-1} + U(\partial_\nu A_\mu)U^{-1} + U A_\mu(\partial_\nu U^{-1})\\ &-\frac{i}{g}\left[
(\partial_\nu\partial_\mu U)+\partial_\mu U\partial_\nu U^{-1}
\right]
\end{align}
$$
and subtracting $b$ from $a$ we get:

$$\begin{align}
F_{\mu\nu} =  & \frac{i}{g}\left[
\partial_\mu U\partial_\nu U^{-1}- \partial_\nu U \partial_\mu U^{-1}
\right]\\
& +(\partial_\mu U)A_\nu U^{-1} - (\partial_\nu A_\mu)U^{-1}\\
& UA_\nu(\partial_\mu U^{-1}) - UA_\mu(\partial_\nu U^{-1})\\
& U(\partial_\mu A_\nu - \partial_\nu A_\mu)U^{-1}
\end{align}
$$
which is neither good looking nor invariant. To make it invariant we add the term $ig[A_\mu, A_\nu]$ that cancels out these unwanted terms when transforming:

$$
F_{\mu\nu} = \partial_\mu A_\nu - \partial_\nu A_\mu -ig[A_\mu, A_\nu]
$$
It is now easy to construct the gauge invariant Lagrangian density for the dynamical part of the gauge field as:

$$
\begin{align}
L_{\text{Gauge}} &= -\frac12\text{Tr}\left(F_{\mu\nu}\cdot F^{\mu\nu}\right) \\
&=-\frac12\sum_{i,j = 1}^3 \text{Tr}\left(
\frac{\tau^i}{2}F^i_{\mu\nu}\frac{\tau^j}{2}F^{j\mu\nu}
\right)\\
&=-\frac14F^i_{\mu\nu}F^{i\mu\nu}
\end{align}
$$
The Yang-Mills Lagrangian, then is:

$$
\begin{align}
L_{\text{YM}} &= L_F + L_{\text{Gauge}}\\
&= \bar\psi(i\gamma^\mu D_\mu - M)\psi -\frac14 F^i_{\mu\nu}F^{i\mu\nu}
\end{align}
$$
Which is invariant under local gauge transformations. Whereas a mass term $m^2 A_\mu A^\mu$ is incompatible with local gauge invariance, so we set the mass to equal zero. The Yang-Mills theory, a non-Abelian gauge theory, differs significantly from Abelian gauge theories like $QED$. 

In this theory self-interactions among gauge fields prevent it from being a free theory even without matter fields. This contrasts with $QED$, where photons do not exhibit self-coupling.

Unfortunately the original form of Yang-Mills theory is not suitable for describing weak interactions. It predicts identical couplings to right and left handed fermions, resulting in parity conservation. 

To maintain gauge invariance, it is crucial to have massless gauge boson, that would lead to weak interactions with an infinite range, similar to $QED$. 

However this contradicts experimental observations. Only by introducing a mass term that breaks the gauge symmetry can the theory be reconciled with experimental results and achieve agreement with reality.


