## Surface Representation
- Formally: Surface is a 2D manifold embedded in 3D space.
- Informally: Surface is boundary of a non-degenerate 3D solid.

A non-degenerate solid object is one where each point can be classified as either interior or exterior.

!!! info "What is a manifold?"
    An n-dimensional manifold will look like an n-dimensional Euclidean space when looked at closely. For example, if you zoom in infinitely on a hollow sphere, it will look like a 2D plane.

### Surface Classifications

| Classification | Examples |
|----------------|-------------|
| Orientable/Non Orientable | Torus is orientable, Klien Bottle is not| 
| Closed/Open | Sphere is closed, Plane is open |
| Manifold/Non-Manifold | Sphere is manifold, Cone is non-manifold |

### Topological Classification
- Topological Equivalence: Two surfaces are topologically equivalent if one can be deformed into the other without any cuts or gluing.
- Genus: Maximum Number of cuttings along non-intersecting closed curves that can be made without separating the surface.

### Operational Classification
- Evaluation: The sampling of the surface geometry or other surface properties.
- Modification: A surface can be changed in terms of geometry(deformations) or topology(cuts, gluing).
- Query: Spacial queries to determine if given point is inside or outside the solid bounded by the surface, or distance of point from the surface.

### Surface Representation
- Implicit Surfaces: Defined as the set of points satisfying an equation $f(x, y, z) = 0$.
- Parametric Surfaces: $S(u, v) = (x(u, v), y(u, v), z(u, v))$ where $S: \mathbb{R}^2 \rightarrow \mathbb{R}^3$.