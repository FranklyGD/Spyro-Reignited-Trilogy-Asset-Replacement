_**This tutorial assumes you already know how to use plugin system, make levels and basic usage of blueprint system.**_



# Introduction:

Now that you populated your map with lighting, fog, and static meshes it's time to spawn actors 

In this guide you're going to learn how to use blueprint system to spawn **actors**,  You can use this guide to spawn not just NPCs but all kinds of actors as well. 



## Problems:

1. Pathfinding for npcs are completely broken, this means they can't walk or move around in your own levels unless you manually move them using blueprints.
2. Some npcs doesn't work at all.
3. Bosses either die in one hit or don't work at all.
4. Some actors like water needs special setup in blueprints in order to work properly.

# Creating A Dummy Enemy Blueprint:
**Create a plugin for the actor you want to spawn**. In my example I’m going to spawn **CES1016_Shepherd**. You can use **UE Viewer aka UModel** to locate your **folder** and **blueprint** names.

![image-20200607044719238](assets/umodelfolder.png)

Replicate the folder structure on your **Unreal project** by creating a new **plugin** and **Blueprints** folder inside the newly created plugin
Inside your **Blueprints** folder create an **Actor** Blueprint Class. Name it the blueprint name you saw on **Umodel**

# Creating Spawner:

Now go to your **Content** folder and create a new **Actor** Blueprint Class. Name it whatever you want. Double click on it to open BP editor and copy the blueprint setup from the image below. 
![](assets/spawner_blueprint_setup.png)

For **Pawn Class** select the dummy **Actor** blueprint you created in my case it’s **BP_CES1016_Shepherd**. Use GetActorLocation** for location and **GetActorRotation** for rotation.

**Compile** and **Save** the blueprint

# Spawning Your Actor:
Place a **Nav Mesh Bounds Volume** to your level and scale it accordingly so it covers your map.
Place the **spawner blueprint** you created to anywhere you want.

**Build** the map and [Cook Content For Windows](https://github.com/FranklyGD/Spyro-Reignited-Trilogy-Asset-Replacement/wiki/Creating-the-Pak-File)