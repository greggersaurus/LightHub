# Introduction

The purpose of this project is to create a model for 3D printing a replacement 
 part for the Light Hub (Atari P/N 000616-01), which is an encoder wheel for
 a 4 inch trackball assembly.

# TODO

1. Narrow the width of the center notch and perform next test print with reduced width center notch.
2. Add details on printer and settings used for test print and details on results.

# Design

An official part was obtained and measured. 

The following are a rough outline of the steps used to model the part in Blender 2.75a:

1. Create a cylinder.
    1. There are 36 raised pillars on outer edge of cylinder.
    2. 432 (36 * 2 * 6) vertices for cylinder, gives each raised and lowered section six faces for rounding the pillars.
2. Duplicate.
3. Shrink and boolean subtract to make outer raise ring.
4. Resize duplicate and boolean union to make inner raise ring.
5. Resize duplicate and subtract to make inner hole.
6. Make cube and union to make inner notch. 
7. Select outer ring face and ctrl-f triangular faces then ctrl -f tris to quad.
8. Select six faces at a time from top of outer ring and extrude to make arms for blocking light.
9. Select vertices of raised arms to round off.

