# Teorema Fundamental del Álgebra

Esquema de una prueba topológica del Teorema Fundamental del Álgebra

"Todo polinomio tiene al menos una raíz en el plano complejo."

- Notar: Polinomios son funciones continuas:


$$ \lim_{z \to z_0} {|P(z) - P(z_0)|} = 0$$

- Definir un conjunto $\mathbf{C}_R = \lbrace z \in \mathbb{C} : |z| = R \rbrace $

- Elegir un Polinomio cualquiera $P$, definido como $P(z) = a_n z^n + a_{n-1} z^{n-1} + \ldots a_0$.

- Notar: Si $a_0 = 0$ entonces el origen es una raíz de $P$ ya que $P(0) = a_n 0^n + a_{n-1} 0^{n-1} + \ldots + 0 = 0$.

- En caso de que $a_0 \neq 0$, considerar $\mathbf{D}_R$ la imagen de $\mathbf{C}_R$ por $P$, es decir $$\mathbf{D}_R = P \left( \mathbf{C}_R \right)$$

- Para valores muy pequeños de $R$, $\mathbf{D}_R$ estará muy próximo a $a_0$, es decir

$$\sup_{z \in \mathbf{C}_R} \lbrace |P(z) - a_0| \rbrace \ \xrightarrow[R \to 0]{} 0$$

- Para valores muy grandes de $R$, el primer término siempre va a terminar dominando ya que

$$\lim_{z \in \mathbf{C}_R\\R \to \infty}
\dfrac{|a_{n-1} z^{n-1} + \ldots + a_0|}{|z^n|} = $$

$$\lim_{ \substack{  z \in \mathbf{C}_R \\ R \to \infty}} |a_{n-1} z^{-1} + \ldots + a_0z^{-n}| = 0 $$

- Entonces para valores muy grandes de $R$ y tomando $$z = R \left( \cos(\theta) + i \sin(theta) \right) $$ $\mathbf{D}_R$ se aproximará como

$$\mathbf{\tilde{D}}_R =  a_n R^n\left( \cos( n \theta) + i \sin(n\theta) \right)$$

que es la imagen de una circunferencia de radio $R^n$ y para valores suficientemente grandes de $R$, esta circunferencia encierra al origen.

- Esquema de la prueba:

- Para $R \rightarrow 0$  la imagen $\mathbf{D}_R$ se condensa en el punto $a_0 \neq 0$.

- Para $R$ muy grande, la imagen $\mathbf{D}_R$ se aproxima a una circunferencia de radio muy grande.

- Como $P$ es continuo, si $R$ varía de valores muy pequeños a muy grandes, en algún valor intermedio la curva $\mathbf{D}_R$ va a tocar el $0$.
                
- Entonces para algún valor de $R$ se cumple que $$P \left( R\cos(\theta) + i R\sin(\theta) \right) = 0$$

- Es decir que $P$ tendrá al menos una raíz!

- Notar que limitándose a los reales este razonamiento deja de ser válido ya que no hay circunferencias en $\mathbb{R}$.
El equivalente de $\mathbf{C}_R$ en $\mathbb{R}$ es el segmento $-R \leq x \leq R$ de $\mathbb{R}$ para el dominio, y el segmento $\min \left( P \left( \mathbf{C}_R \right) \right) \leq y \leq \max \left( P \left( \mathbf{C}_R \right) \right)$ de $\mathbb{R}$ para el codominio.
Según sean los coeficientes de $P$ se puede dar que $\min \left( P \left( \mathbf{C}_R \right) \right) > 0$  $\forall R \in \mathbb{R}$ (o bien $\max \left( P \left( \mathbf{C}_R \right) \right) < 0$  $\forall R \in \mathbb{R}$) y luego $P$ no se anule en ningún punto de $\mathbb{R}$.
