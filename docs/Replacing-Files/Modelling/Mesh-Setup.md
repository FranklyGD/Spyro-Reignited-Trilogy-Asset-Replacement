------

## Requirements:

### Modelling Related Tools
* [Blender](https://www.blender.org/download/)
* * [Blender PSK/PSA Importer 2.8](https://github.com/Befzz/blender3d_import_psk_psa/raw/latest/addons/io_import_scene_unreal_psa_psk_280.py)
* * [Blender PSK/PSA Importer 2.7](https://github.com/Befzz/blender3d_import_psk_psa/raw/latest/addons/io_import_scene_unreal_psa_psk_270.py)
* [3DS Max](https://www.autodesk.com/products/3ds-max/overview)
* * [3DS Max PSK/PSA Importer](https://www.gildor.org/projects/unactorx)



## [Importing - Exporting Your Mesh](Import-Export-Settings.md) 

------

There really is no point on showing you series of images about how to import-export a mesh into your 3d editor.
**That page explains the correct import-export settings to use when importing a model to get the best results**

## Static Meshes

------

Basic objects in the game, such as rocks, buildings.

There is no setup required for static meshes. Import to Unreal and [replicate the file stucture in Unreal.](../../Preparing-Modding/Replicating-the-Game-Structure-Unreal.md) 

By default, when you import a static mesh into Unreal Engine Editor, it would either come with materials set to default white or none at all (usually seen as a gray grid texture). You may add and setup these materials however you like to appear in the game.



## Skeletal Meshes  

------

As it's name implies, they are meshes for character or objects that can be animated.


## Skeletal Mesh Setup

After you finished your modelling and imported the model/skeleton accordingly with the import-export settings. There are few things that need to be done in order to have error-free replacement.

1. Make sure your armature name is `Armature` **with capital A.**

2. After importing to Unreal follow [Replicating Game Structure](../../Preparing-Modding/Replicating-the-Game-Structure-Unreal.md) page to place your mesh into correct folder.

3. Check the skeleton,physics asset and skeletal mesh **names** and **locations** are correct. [(Replicating game structure)](../../Preparing-Modding/Replicating-the-Game-Structure-Unreal.md)

4. Click on the skeleton and check the root bone's scale, It needs to be 1.

5. Having more separated meshes seems to cause fatal errors in the game, make sure you merge your meshes before exporting.

   
   
   Depending on the mesh, you will need to remove physics and skeleton assets in u4pak process.
   
   
   
   | Character |             Requires Deletion In Paking Process              | Requires Replacing Of All Animations |
   | :-------: | :----------------------------------------------------------: | :----------------------------------: |
   |   Spyro   |                             Yes                              |                  No                  |
   |  Sheila   | No but requires [sockets](Socket-Names.md) to have attacks work correctly. |                  No                  |
   |   Elora   | No but skeleton import with umodel have bad bone locations. [Use Elora Workspace](https://github.com/Magic-Nipples/SRT-Workspace_Elora-Asset-Swap) for fixed bones. |                 Yes                  |
   
   


## Skeleton Replacement (Advanced, Untested)

If you're planning on replacing the skeleton itself as well as the model follow the guidelines below to have crash and bug free replacement:

- Make sure bone names are exactly named like how they are in Reignited. Some bones are used by animation blueprints and if said bones cannot be found game will crash.

- Some models needs [sockets](Socket-Names.md) to work correctly, for example Spyro's breath comes out from a socket attached to the head bone. 

##Common Issues

### Root bone's scale being 100 in Unreal Engine:

1. Open blender, scale both your mesh and skeleton 100 times
2. Apply scales (ctrl+a)
3. Scale model down to 0.01
4. Export **without applying scale**

!!! tip
	If scale is 0.01 instead of 100, do the same steps but opposite scales.

### Making Metal Heat Effect Work Again On Enemies

TODO: Explain more

In order to fix metal heat up effect you need to use vertex colors. Use Green vertex color on where you want meshes to have heat up effect.

### Materials For Meshes

Some materials are special that they have parameters which are modified at run-time]  or are usually not loaded by default and swapped in later by an in-game event. **Similar to any other asset, before cooking just make sure the name of the file is the same as Umodel Viewer.**