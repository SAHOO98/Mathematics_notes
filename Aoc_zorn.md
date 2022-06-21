# Definition of AOC
Let $\mathcal{A}$ be a non-empty collection of non-empty sets. A function $f : \mathcal{A}\rightarrow \cup\mathcal{A}$ is called a **choice function for $\mathcal{A}$** if $f(A) \in A$ for all $A \in \mathcal{A}$.

Or more compactly.
$$\forall \mathcal{A} [\emptyset \notin \mathcal{A} \implies \exists f : \mathcal{A} \rightarrow \cup \mathcal{A},\text{ } \forall A \in \mathcal{A} (f(A)\in A) ]$$

# Partial Ordered set(POSET):
Let  $P\neq \emptyset$. Then $(P, \le)$ is poset if:
* (Reflexive) $x\le x$ $\forall x \in P$
* (Antisymmetric) $x\le y$ and $y \le x$ then $x=y$  $\forall x,y \in P$
* (Transitive) $x\le y$ and $y \le z$ then $x\le y$  $\forall x,y,z \in P$

$\le$ will be called total order when every element of $P$ is comparable.

# Upper bound and lower bound
Let $(P, \le)$ be a POSET. Let $A \subseteq P$.
* $p\in P$ is an **upper bound** of A if and only if for all $a \in A$, $a\le p$.
* $p\in P$ is an **lower bound** of A if and only if for all $a \in A$, $p\le a$.

## Least Upper bound and Greatest Lower Bound

* **LUB property:** If a subset of a poset is bounded above then there will always exist a least upper bound(LUB)(supremum) of that subset.

* **GLB property:** If a subset of a poset is bounded below then there will always exist a greatest lower bound(GLB)(infimum) of that subset.

# Maximal and minimal element
Let $(P, \le)$ be a POSET. Let $A \subseteq P$.
* **Maximal element of A**: $m \in A$ is a maximal element of $A$ if $p\in A$ satisfies $m\le p$ then $m=p$. Another way of saying is "nothing is bigger than $m$ in A". ($\nexists y \in A$ s.t $m\le y$ and $m \neq y$)

* **Minimal element of A**: $m \in A$ is a manimal element of $A$ if $p\in A$ satisfies $p\le m$ then $m=p$. Another way of saying is "nothing is smaller than $m$ in A". ($\nexists y \in A$ s.t $y\le m$ and $m \neq y$)

# Greatest element and Least element
Let $(P, \le)$ be a POSET. Let $A \subseteq P$.

* **Greatest Element:**  $g \in P$ is the greatest element of of $A$ if  $g \in A$ satisfies $a \le g$ for all $a \in A$. 
* **Least Element:**  $g \in P$ is the least element of of $A$ if  $g \in A$ satisfies $g \le a$ for all $a \in A$. 


# Zorn's Lemma
Let $(P, \le)$ be a non-empty partial order such that every chain(Total ordered subset of P)
in $P$ has an upper bound then P has a maximal element.

