## Basic Mapping
Let us have a 2D Hilbert space with two complex vectors $a + bi, c + di$.

$$
V = \begin{pmatrix}
a + bi \\
c + di
\end{pmatrix}
= \begin{pmatrix}
r_1 e^{i\phi_1} \\
r_2 e^{i\phi_2}
\end{pmatrix}
$$

To convert this to a point on the Bloch sphere, we first convert it to its polar form and then write it as coefficients of, say, $|0\rangle$ and $|1\rangle$.

$$
|\psi\rangle = r_1 e^{i\phi_1} |0\rangle + r_2 e^{i\phi_2} |1\rangle
$$

We don't care about the exact phase, so we can write $\phi_2$ relative to $\phi_1$ and get rid of $\phi_1$. At the same time, we normalize $r_1$ and $r_2$.

$$
|\psi\rangle = \frac{r_1}{\sqrt{r_1^2 + r_2^2}} |0\rangle + \frac{r_2}{\sqrt{r_1^2 + r_2^2}} e^{i(\phi_2 - \phi_1)} |1\rangle
$$

Normalized $r_1, r_2$ are conveniently angles on a triangle:

$$
|\psi\rangle = \cos(\theta) |0\rangle + e^{i\phi} \sin(\theta) |1\rangle
$$


## Mapping $\mathbb{S}^2$ to the Bloch sphere

### Preliminaries: n-Sphere
Consider a 3-d ball and it's boundary. The boundary is a 2-sphere, denoted by $\mathbb{S}^2$. The 2-sphere is a 2-dimensional manifold embedded in 3-dimensional Euclidean space.

![2-sphere](https://upload.wikimedia.org/wikipedia/commons/thumb/7/7e/Sphere_wireframe_10deg_6r.svg/220px-Sphere_wireframe_10deg_6r.svg.png)

We know we can parametrize this sphere generally as $(x- x_0)^2 + (y - y_0)^2 + (z - z_0)^2 = r^2$, or more generally $\mathbb{S}^2: (x_0 - c_0)^2 + (x_1 - c_1)^2 + (x_2 - c_2)^2 = r^2 \in \mathbb{R}^3$. This is a 2-sphere in 3-d space.

We can go one level up and write $\mathbb{S}^3: \sum_{i=0}^{3} (x_i - c_i)^2 = (x_0 - c_0)^2 + (x_1 - c_1)^2 + (x_2 - c_2)^2 + (x_3 - c_3)^2 = r^2 \in \mathbb{R}^4$. This is a 3-sphere in 4-d space.

### Preliminaries: Quantum States

We we have two vectors say $v,w$ in the Hilbert Space $\mathbb{C}^2$ such that $v = \begin{pmatrix} v_0 \\ v_1 \end{pmatrix}$ and $w = \begin{pmatrix} w_0 \\ w_1 \end{pmatrix}$, such that inner product is defined as $\langle v, w \rangle = v^\dagger w = v_0^* w_0 + v_1^* w_1$.

We define such vectors as quantum states. A pure state as a consequence is when $||v|| = 1$. We tend to write such states with their orthonormal bases $|0\rangle, |1\rangle$ as

$$
|\psi\rangle = \alpha |0\rangle + \beta |1\rangle \because \alpha^2 + \beta^2 = 1
$$


### Combining the two
Cll the elements of $\mathbb{C}^2$ as $v = \begin{pmatrix} v_0 \\ v_1 \end{pmatrix}$, such that $||v|| = 1$. One can imagine that since we have now eliminated one dimension by normalising our state, we can map this to a 3-sphere inside 4-d space.
