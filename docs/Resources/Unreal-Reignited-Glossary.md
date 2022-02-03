
## Known Texture Name Meaning

Suffixes:  
* `_C` is Colour/Diffuse/Albedo  
* `_M` is Metallic  
*  `_F` is Fuzziness Mask  
* `_T` is Translucency (for subsurface)  
* `_N` is Normal  
* `_R` is Roughness  
* `_ARM` is a composite map consisting of  Ambient Occlusion, roughness and metallic on RGB channels respectively.  
* `_ORM` is a composite map consisting of  Ambient Occlusion, roughness and metallic on RGB channels respectively.  
* `_Body_Mask` is the mask used in most emissive (power up) textures  

| Texture Suffix | Red Channel Purpose | Green Channel Purpose | Blue Channel Purpose | Alpha Channel Purpose |
| -------------- | ------------------- | --------------------- | -------------------- | --------------------- |
| _ARME          | Ambient Occlusion   | Roughness             | Metallic             | Emission              |
| _ORM           | Ambient Occlusion   | Roughness             | Metallic             | N/A                   |
| _RMSE          | Roughness           | Metallic              | Speculars            | Emission              |


## Meshes

* `SK` Skeletal Mesh:  **Model** itself, you can change which skeleton it uses or change/add materials. It doesn't contain animations or skeleton itself.
* `SKEL` Skeleton: Skeleton used by model. Some models have shared skeletons like dragon elders. Sockets can be created from this file
* `PH` Physics Asset: Used for defining physics and collision for skeletal mesh, think it like a hitbox but it's not used in Spyro Reignited Trilogy

## Materials

- `MF` Material Function: Little snippets of material graphs that can be reused across multiple materials.	
- `M` Material: Main materials, think of them as shaders from Unity
- `MI` Materian Instances: Instances of materials, they do not allow anything other thhan changing already defined parameters from it's parent material, Think of it as materials that use a shader in Unity.

