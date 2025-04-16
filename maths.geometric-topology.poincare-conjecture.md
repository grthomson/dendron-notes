---
id: 81tfolv0ye1e6yx4zdp51ft
title: Poincare Conjecture
desc: ''
updated: 1744807458831
created: 1744804328676
---
# "Every closed smooth simply connected 3-manifold is diffeomorphic to S^(3)"

###  NB :
- Every topological 3-manifold can be equipped with a differentiable structure
- Every homeomorphism between smooth 3-manifolds can be approximated by a diffeomorphism
- Therefore statements about topological 3-manifolds up to homeomorphism are requivalent to statements about smooth 3-manifolds up to diffeomorphism

### A 3-manifold is a topological space 𝑀 such that every point has a neighborhood 𝑈 ⊂ 𝑀 which is homeomorphic to an open subset of 𝑅 3. 
- That is, ∀ 𝑝 ∈ 𝑀 there exists an open neighborhood 𝑈 of 𝑝 which admits a homeomorphism 𝜑 : 𝑈 → 𝑉 ⊂ 𝑅 3

### A topological manifold isn't necessarily give a differentiable or smooth manifold - we need the transition maps for overlapping charts to be smooth

- A topological manifold has charts 𝜙_𝑖 : 𝑈_𝑖 → 𝑅^𝑛 where each 𝜙_𝑖 is just a homeomorphism (continuous, with continuous inverse). The transition maps 𝜙_𝑗 ∘ 𝜙_𝑖^−1 ϕ j ​are homeomorphisms between open subsets of 𝑅^𝑛, but not necessarily smooth.

- We have a smooth manifold when the transition maps 𝜙_𝑗 ∘ 𝜙_𝑖^(−1) are all smooth wherever charts overlap.

### In dimension 3 it's always possible to find an atlas (a collection of charts) whose transition maps are smooth — i.e., you can promote the topological manifold to a smooth one.

### But this is nontrivial, and fails in other dimensions:

- In dimension 4 there are topological manifolds that do not admit any smooth structure at all. 

- In dimension 7+ some topological manifolds admit multiple inequivalent smooth structures (same underlying topology, different ways to define smoothness — e.g. exotic 𝑅^4).

### When is a manifold homeomorphic to a subset of 𝑅^𝑛? 

- Embedding: A manifold 𝑀 is said to be embedded in 𝑅^𝑁 if there is a smooth injective map 𝑓 : 𝑀 ↪ 𝑅^𝑁 whose image is homeomorphic (and diffeomorphic) to 𝑀, and which has an injective derivative everywhere. 
- Whitney's Embedding Theorem says that: Any smooth 𝑛-dimensional manifold can be embedded into 𝑅^2𝑛 R. So yes, eventually you can embed it into some big Euclidean space — just not necessarily in dimension 𝑛.