**Q:My texture is white**  
A:Make sure you are using **cooked** assets and not source assets, cooked assets can be found in `<Project>/Saved/Cooked/WindowsNoEditor/<Project-Name-Again>/`

**Q:I replaced materials and now I have a grid texture instead.**  
A:Unreal Engine 4 have a function called Material Flags, these are used for optimization purposes, enable the correct option that your material uses. You can find more information in here: https://docs.unrealengine.com/en-US/Engine/Rendering/Materials/MaterialProperties/index.html#usage

**Q:Reignited crashes after replacing some stuff with my own mods.**
A:This can be due to many issues,  making sure your unreal engine version is 4.19.2 and if it's a model replacement making sure entire model is merged into one is a good start.

**Q:My model looks like a popsicle**  
* Make sure you renamed your skeleton to `Armature` with capital A before importing it to Unreal Editor. 
* Another important part is to check for bone scales in Blender and Unreal Editor. **In Unreal Engine main bone scale needs to be 1**
* For some models you need to remove SKEL_ files in u4pak process.

**Q:My model is T-Posing in game **  
A:Make sure skeleton and physics assets are named exactly like original ones you're going to replace.

**Q:Model resizes itself when playing animation **  
A:Make sure model's skeleton is sized correctly, if your model looks huge in Unreal Editor page.

**Q:My replacement doesn't show up in the game**  
A:Make sure you replicated game structure in [Unreal Editor](Preparing-Modding/Replicating-the-Game-Structure-Unreal.md) and in [U4PAK](Pak-Files/Replicating-the-Game-Structure-U4Pak.md).

**Q:My assets doesn't show up in cooked folder**  
A:Make sure you saved them in the Unreal Editor first, if you see a star shape at the left bottom of the asset's thumbnail it means it's not saved yet and will not be cooked.

**Q:Deleting and empty folder in Unreal prompts references window.**
A:Use [Fixup Redirector From Editor](ttps://docs.unrealengine.com/en-US/ProductionPipelines/Redirectors/index.html).

**Q:Installed mod doesn't work. **  
A:**Make sure you're using `~mods` folder** to install your mods, placing mods in your Paks folder **IS NOT RECOMMENDED** and some mods **ARE NOT GOING TO WORK**.

**Q:My sound replacements don't play.**  
A:Try changing **Vorbis Quality** to **Low** or **Medium**

**Q:Files doesn't show up in cooked folder**
A:Make sure your files are saved first(no * symbol on thumbnails)

