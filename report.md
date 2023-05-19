# Bachelor Project Report

## Week 1

- Forked and cloned the repo
- Got accustomed to the code
    - Look up cairo tutorials to understand wtf is going on

## Week 2
- Started coding
    - `polygons.h` and `polygons.cc`
    - `polygons_generator.h` and `polygons_generator.cc`
    - `matrix.h`

### Polygons properties
- points (`std::vector<vec2d>`): the points that form the polygon, **in local
    coordinates**;
- center (`vec2d`): where the origin of the local coordinates lies in global
    coordinates;
- angle (`double`): how the points are rotate around the origin (to keep always
    the same points but rotating them when making computations are drawing)
    **interesting question for later: does computing the points rotated at each
    iteration less computationally efficient than just storing them each time
    the angle changes?**.

### Polygon Generator
To make life easier for testing different cases, I made a generator of polygons
that for now is able to generate any triangle and any rectangle. Simple shapes
but that are simple enough to understand what happens when they get hit. We'll
then see if the calculation for the forces transpose to any arbitrary polygon.
