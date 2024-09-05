## Types of Projections

- Orthographic/Parallel: projection lines are all parallel to each other (direction of projection or DOP)
- Perspective: projection lines converge at a single point (center of projection or COP)

<figure markdown="span">
    ![Perspective vs Orthographic Projection](images/perspective_parallel_views.png){ width="800" }
  <figcaption>Perspective vs Orthographic Projection</figcaption>
</figure>

!!! note
    There are many types of projections, but all of them can be classified into these two categories.

    There are many more subtypes of Parallel projection than Perspective projection.

## Parallel Projections

In the given figure, DOP is the direction of projection and VPN is view plane normal. Assume object face of interest lies in principal plane.

<figure markdown="span">
    ![Types of Parallel Projections](images/parallel_projections.png){ width="800" }
  <figcaption>Types of Parallel Projections</figcaption>
</figure>

| Type | Description | VPN $\parallel$ a principal axis? | DOP $\parallel$ VPN? |
|------|-------------|-----------------------------------|----------------------|
| Multiview Orthographic | Shows a single face, exact measurements | Yes | Yes |
| Axonometric | Adjacent faces, ==none exact==, uniformly foreshortened | No | Yes |
| Oblique | adjacent faces, ==one exact==, others uniformly foreshortened | Yes | No |

???+ note "What the hell is foreshortening?"
    Foreshortening is the visual effect or optical illusion that causes an object or distance to appear shorter than it actually is because it is angled toward the viewer.

### Multiview Orthographic Projections
- Projectors are orthogonal to the projection plane
- Projection plane is parallel to one of the principal planes
- Think of taking front view, top view, and side view of an object

### Axonometric Projections

<figure markdown="span">
    ![Types of Axonometric Projections](images/axonometric_projections.png){ width="800" }
    <figcaption>Different types of Axonometric Projections</figcaption>
</figure>

<div class="center-table" markdown>

| Type | Description  <img width=300/>|
|------|------------- |
| Isometric | All three principal axes equal ($120^\circ$) |
| Dimetric | Two principal axes are equal |
| Trimetric | All three principal axes are different |

</div>

> Skipping Oblique Projections for now.

## Perspective Projections

- Describes the way we see the world
- Parallel lines don't remain parallel post projection (Foreshortening is not uniform)
- ==View Point== is the point from which the object is viewed. It's an actual point
- ==Vanishing Points== are points where parallel lines converge. They are imaginary points.

<figure markdown="span">
    ![Perspective Projections](images/perspective_projection.svg){ width="800" }
    <figcaption>Perspective Projections</figcaption>
</figure>

| Type | Description |
|------|-------------|
| One-point Perspective | All parallel lines converge to a single point |
| Two-point Perspective | All parallel lines converge to one of two points |
| Three-point Perspective | All parallel lines converge to one of three points |

There can be more than three vanishing points as well, and that would be an N-point perspective.