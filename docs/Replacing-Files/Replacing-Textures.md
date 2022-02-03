

# Requirements:

------



- Unreal Engine 4.19.2

- Modified texture you're going to replace



#Steps By Step Importing A Texture To Unreal Engine
Todo Add images maybe?

1. First step is  [Replicating The Game Structure For Unreal Engine](../Preparing-Modding/Replicating-the-Game-Structure-Unreal.md) ,

2. [Next import your texture to Unreal.](https://docs.unrealengine.com/en-US/RenderingAndGraphics/Textures/Importing/index.html)

3. Continuing from Replicating The Game Structure For Unreal Engine page, make sure you texture name and location is replicated correctly

4. [Cook Content For Windows.](../Pak-Files/Cooking-Unreal-Files.md) 

5. [Pak File Creation and Replicating Game Structure In U4PAK](../Pak-Files/Replicating-the-Game-Structure-U4Pak.md) 



## Known Texture Name Prefixes

Suffixes:  
* `_C` is Color/Diffuse/Albedo  
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



## Editing Softwares

**Alpha channels on textures used for a lot different purposes**  one  example is Spyro's eye texture. **Alpha channel of the eye texture is used for adding an eye glint. It is recommended to have a software that can edit or *temporarily* alpha channel.**

GIMP: https://www.gimp.org/downloads/    
Krita: https://krita.org/en/download/krita-desktop/