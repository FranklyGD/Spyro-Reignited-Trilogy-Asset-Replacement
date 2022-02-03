## 3DS Max 2019
* PSK Importer ([Download Here](https://www.gildor.org/projects/unactorx))
    - Settings
        - Default (You don't need to change anything)
* FBX Exporter
    - Settings
        - Default (You don't need to change anything)

## Blender
* PSK Importer ([Download Here](https://github.com/Befzz/blender3d_import_psk_psa))
    - Settings
        - Default (You don't need to change anything)
* Mesh/Armature (Only Root Object)
    - Position: Origin (0.0 XYZ)
    - Scale: Unscaled (1.0 XYZ)
    - Rotation: Unrotated (0.0 XYZ)
* FBX Exporter (If there is an armature, make sure it is named `Armature`)
    - Main
        - Scale: 1.00
        - Only Armature and Mesh
    - Geometry
        - Apply Modifiers: Enabled (Only needed if there are extra modifiers than Armature)
        - Smoothing: Face
        - Tangent Space: Enabled
    - Armatures
        - Add Leaf Bones: Disabled
    - Mesh Armature Name: Armature

## Blender for Unreal Engine Addon

This wasn't tested by any of us but looking at Unreal Engine Forums people seems to be getting betting results compared to default FBX exporter.

https://github.com/xavier150/Blender-For-UnrealEngine-Addons

## Unreal
* Unreal FBX Importer
    - Mesh
        - Skeletal Mesh: Enabled
        - Import Mesh: Enabled
        - Normal Import Method: Normals and Tangents
    - Transform
        - Import Uniform Scale: 1.0
    - Miscellaneous
        - Convert Scene: Enabled
        - Force Front XAxis: Disabled
        - Convert Scene Unit: Disabled
    - Material
        - Import Materials: Enabled
        - Import Textures: Enabled
