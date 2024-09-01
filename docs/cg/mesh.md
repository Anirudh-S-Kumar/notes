## Introduction to Mesh and it's properties
Piecewise linear approximation with error $O(h^2)$ is called a mesh

<figure markdown="span">
  ![Convex Hull](images/mesh.png){ width="300"}
  <figcaption>Convex Hull (the boundary is P0 P1 P2 P3)</figcaption>
</figure>

Mesh elements

- Face: Subset of a 3d plane
- Edge: Incident points of 2 or more faces
- Vertex: Incident points of 2 or more edges 

Mesh Local Structure

- ==Element type==: Triangle, Quad meshes, or polygon meshes. We always use triangles as they are always planar.
- ==Element shape==: Isotropic, i.e. locally uniform in all directions, or anisotropic, i.e. non-uniform in all directions.
- ==Element density==: Uniform or non-uniform. Non-uniform density is used to refine the mesh in regions of interest.

!!! note
    For better illustrations, see lecture slides on google classroom. I might add some illustrations here in the future myself but for now, I will just leave it as it is.

Regularity of Mesh

- Irregular: any number of irregular vertices
- Semi-regular: small number of irregular vertices
- Highly regular: most vertices are regular
- Regular: all vertices are regular

!!! info
    A Vertex is regular if it is incident to 6 edges. We generally use regular meshes as they are easier to work with.

## Mesh Data Structures
