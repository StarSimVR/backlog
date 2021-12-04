<!--
    REFERENCE.md : important information regarding this project.

    See `LICENSE' for full license.
-->

<!--
    Copyright (C) 2021 Kevin Matthes, Luka-sama and Niklas Leukroth

    This program is free software; you can redistribute it and/or modify
    it under the terms of the GNU General Public License as published by
    the Free Software Foundation; either version 2 of the License, or
    (at your option) any later version.

    This program is distributed in the hope that it will be useful,
    but WITHOUT ANY WARRANTY; without even the implied warranty of
    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
    GNU General Public License for more details.

    You should have received a copy of the GNU General Public License along
    with this program; if not, write to the Free Software Foundation, Inc.,
    51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA.
-->

<!----------------------------------------------------------------------------->

# Reference

## Godot

### Up vector
Godot has Y-axis as up vector.  Please mind this when exporting your geometry.

### Supported file types for geometry
glTF 2.0, DAE (COLLADA), OBJ (Wavefront), ESCN, FBX

We use in this project glTF 2.0 and OBJ (Wavefront).

### Supported file types for textures
.bmp, .dds, .exr, .hdr, .jpg (.jpeg), .png, .tga, .svg, .svgz, .webp

In glTF 2.0 (.glb) you can also add texture directly to the model.

### Procedural textures
You can use [this tool](https://github.com/RodZill4/material-maker) to create procedural textures. It generates all necessary files to use procedural textures in Godot.

### VR support
To add VR support, you should:

* Add addon (e. g. OpenVR)
* Add ARVROrigin node with ARVRCamera and two ARVRControllers (left and right) as children
* Add scripts to ARVR-nodes

Note that in VR 1 unit = 1 meter in the real world. Remember this creating your 3D models.

See [Godot Docs](https://docs.godotengine.org/de/stable/tutorials/vr/index.html) for details.
