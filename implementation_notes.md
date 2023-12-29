# Transformations

As the OpenGL takes Cartesian coords as an input (3D Euclidean space, further referred as E3), the following transformations have to be done, the curved space has to be first projected onto the E3. The projection should conserve the spherical coordinates relative to the camera.

Required transformations are.
1. Object local coords -> world coords
2. -> world coords with origin in camera
3. -> spherical coords with origin in camera
4. -> 3E world coords with origin in camera
5. -> 3E world coords
6. -> local coords in 3E

Altough the process can be for some cases of curved spaces simplified and some of these transformations eliminates (https://citeseerx.ist.psu.edu/document?repid=rep1&type=pdf&doi=8a6891c95d6e6ef480460b5af67c69cfb7d0ceea), this optimization is left for later development and here, I will proceed with this (naive) approach.

