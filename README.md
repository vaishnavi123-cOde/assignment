# 3D Mesh Generator

This Python script generates 3D meshes for two simple objects: a pillow and a ball. The meshes are saved in Wavefront OBJ format.

## Features

- Creates a pillow mesh with a curved top surface and flat bottom
- Creates a spherical ball mesh
- Exports meshes to standard OBJ format
- Configurable parameters for size and resolution

## Generated Meshes

1. Pillow (outputs/pillow.obj):
   - Dimensions: 2.0 x 0.5 x 1.5 (width x height x depth)
   - Vertices: 800
   - Faces: 1,444
   - Features a subtle bulge in the middle for realistic pillow effect

2. Ball (outputs/ball.obj):
   - Radius: 1.0
   - Vertices: 400
   - Faces: 722
   - Perfect sphere generated using spherical coordinates

## Functions

- `create_pillow_mesh(width=2.0, height=0.5, depth=1.5, resolution=20)`
- `create_ball_mesh(radius=1.0, resolution=20)`
- `save_obj(vertices, faces, filename)`

## Output Format

The meshes are saved in standard OBJ format:
- Vertices are defined with 'v' followed by x, y, z coordinates
- Faces are defined with 'f' followed by vertex indices (1-based)

## Dependencies

- NumPy
- os (standard library)
