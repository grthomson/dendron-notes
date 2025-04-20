---
id: 81tfolv0ye1e6yx4zdp51ft
title: Poincare Conjecture
desc: ''
updated: 1745152271410
created: 1744804328676
---
# "Every closed smooth simply connected 3-manifold is diffeomorphic to S^(3)"

###  NB :
- Every topological 3-manifold can be equipped with a differentiable structure
- Every homeomorphism between smooth 3-manifolds can be approximated by a diffeomorphism
- Therefore statements about topological 3-manifolds up to homeomorphism are equivalent to statements about smooth 3-manifolds up to diffeomorphism

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

## Fibre Bundles

A fibre bundle is a quadruple ( 𝐸 , 𝑀 , 𝜋 , 𝐹 ) where: 

- 𝐸 (total space), 𝑀 (base space), and 𝐹 (fibre) are topological spaces, 
- 𝜋 : 𝐸 → 𝑀 is a continuous surjection, 
- For every 𝑝 ∈ 𝑀, there exists an open set 𝑈 ∋ 𝑝 and a homeomorphism 

𝜙 : 𝜋^(−1)(𝑈) → 𝑈 × 𝐹 

such that 𝜋 = pr_1 ∘ 𝜙. 

This expresses that: 𝜋^(− 1)( 𝑈 ) ≅ 𝑈 × 𝐹,  i.e. the bundle is locally a product space.

```
           φ
π⁻¹(U) ---------> U × F
  |                 |
  | π               | pr₁
  v                 v
   U  ----------->  U
          id
```

In simple terms we have a continuous surjection 𝜋 : E --> M and for any point in M, there is *some* containing open set U whose pre-image under 𝜋 is homoeomorphic to the product of U with F.

The product of open sets in M with the fibre F captures the "local product" aspect of E. Note that 𝜙 is a homeomorphism between U x F (in M x F) and 𝜋^(−1)(𝑈) (open in E).

### Example 1: Möbius Band 

We define the Möbius band as the quotient space: 

### 𝐸 : = ( [ 0 , 1 ] × 𝑅 ) / ∼ 
 with the equivalence relation: 
( 0 , 𝑦 ) ∼ ( 1 , − 𝑦 ) 


- Total space: Möbius band 𝐸 
- Base space: 𝑀 = 𝑆^1 (the circle) 
- Fibre: 𝐹 = 𝑅 

### Projection Map π
Define:
-  π: E → S¹
- π([x, y]) := x mod 1

This is well-defined because:

If (0, y) ∼ (1, –y), then x mod 1 gives the same point in S¹ = ℝ / ℤ.

So π is a continuous surjection, sending each fibre (a vertical line) to a point on the base circle.

Local Trivializations
Choose an open interval U ⊂ S¹ that avoids the gluing point (e.g., a small arc not containing the image of x = 0 or x = 1).

Then: π⁻¹(U) ⊂ E is homeomorphic to U × ℝ

This is because the gluing does not affect these interior regions.

Define the trivialization:

φ: π⁻¹(U) → U × ℝ
φ([x, y]) = (x mod 1, y)

### The circle S¹ is defined as ℝ / ℤ, so x mod 1 gives a point on the circle.

The projection π([x, y]) = x mod 1 sends each point on the Möbius band to its basepoint on S¹.

Over small open intervals in S¹, the Möbius band looks like a rectangle (no twist), so:


π⁻¹(U) ≅ U × ℝ
via the map φ([x, y]) = (x mod 1, y) — a homeomorphism.

This map is a homeomorphism

- E Locally: 𝜋^(−1) ( 𝑈 ) ≅ 𝑈 × 𝑅 for small open 𝑈 ⊂ 𝑆^1. 
- Globally: The bundle is not homeomorphic to 𝑆^1 × 𝑅 due to a twist in how fibres are glued around the circle. This is a nontrivial line bundle. 

### Example 2: Tangent Bundle of 𝑆 ^ 1 (The Circle)
- Total space: 𝑇𝑆^1 ≅ 𝑆^1 × 𝑅 
- Base space: 𝑀 = 𝑆 1 
- Fibre: 𝐹 = 𝑅 

- 𝑇𝑆^1 Locally: 𝜋 − 1 ( 𝑈 ) ≅ 𝑈 × 𝑅 
- Globally: In this case, the bundle is globally trivial — the tangent bundle of the circle is diffeomorphic to the cylinder 𝑆 1 × 𝑅. This is a trivial line bundle.
In other words the product of the fibre and base space just IS the total space E.