| Command                | Value | Effect                    |
| ---------------------- | --------------- | ------------------------- |
| r.PostProcessAAQuality | `0-6`       | Anti Aliasing Quality     |
| r.SkeletalMeshLODBias  | `0-4`       | Skeletal Mesh LOD Quality |
| r.ViewDistanceScale    | `0.01-10`   |                           |


## Shadow Quality

| Command |Value             |Effect                       |
|-----------------------------------------------|-------------------|-----------------------------|
|r.LightFunctionQuality              			|`0-1`				|                             |
|r.ShadowQuality                     			|`0-5`				|                             |
|r.Shadow.CSM.MaxCascades            			|`1-10`				|                             |
|r.Shadow.MaxResolution              			|`512-4096`			|                             |
|r.Shadow.MaxCSMResolution           			|`512-4096`			|                             |
|r.Shadow.RadiusThreshold            			|`0-0.06`			|                             |
|r.Shadow.DistanceScale				 			|`0.4-1.0`			|                             |
|r.Shadow.CSM.TransitionScale        			|`0-1.0`			|                             |
|r.Shadow.PreShadowResolutionFactor  			|`0.5-1.0`			|                             |
|r.DistanceFieldShadowing            			|`0-1`				|                             |
|r.DistanceFieldAO                   			|`0-1`				|                             |
|r.VolumetricFog                     			|`0-1`				|                             |
|r.VolumetricFog.GridPixelSize       			|`4-16`				|                             |
|r.VolumetricFog.GridSizeZ           			|`64-128`			|                             |
|r.VolumetricFog.HistoryMissSupersampleCount	|`4-16`				|                             |
|r.LightMaxDrawDistanceScale         			|`0-1`				|                             |
|r.CapsuleShadows                    			|`0-1`				|                             |


## PostProcess Quality 
| Command |Values      |Effect                       |
|---------------------------------------|------------|-----------------------------|
|r.MotionBlurQuality					|`0-4`       |        |
|                                |`1-0.4`     |                             |
|r.AmbientOcclusionMaxQuality			|`0-100`     |                             |
|r.AmbientOcclusionLevels				|`0 - -1`    |                             |
|r.AmbientOcclusionRadiusScale			|`1.2-1.0`   |                             |
|r.DepthOfFieldQuality					|`0-4`       |                             |
|r.RenderTargetPoolMin					|`300-1000`  |                             |
|r.LensFlareQuality						|`0-3`       |                             |
|r.SceneColorFringeQuality				|`0-1`       |                             |
|r.EyeAdaptationQuality					|`0-2`       |                             |
|r.BloomQuality							|`0-5`       |                             |
|r.FastBlurThreshold					|`100`        |                             |
|r.Upscale.Quality						|`0-100`     |                             |
|r.Tonemapper.GrainQuantization			|`0-1`       |                             |
|r.LightShaftQuality					|`0-1`       |                             |
|r.Filter.SizeScale						|`0.6-1`     |                             |
|r.Tonemapper.Quality					|`0-5`       |                             |

## Texture Quality
| Command |Value      |Effect                       |
|-----------------------------------|------------|-----------------------------|
|r.Streaming.MipBias				|`0-1.5`     ||
|r.MaxAnisotropy					|`0-8`       ||
|r.Streaming.LimitPoolSizeToVRAM	|`0-1`       ||
|r.Streaming.PoolSize				|`400-3000`  ||
|r.Streaming.MaxEffectiveScreenSize	|`0`         ||

## Effects Quality
| Command |Value      |Effect                        |
|-----------------------------------|-----------|-------------------------------|
|r.TranslucencyLightingVolumeDim	|`24-64`    |                               |
|r.RefractionQuality				|`0-2`      |                               |
|r.SSR.Quality						|`0-4`      |                               |
|r.SceneColorFormat					|`0-4`      |                               |
|r.DetailMode						|`0-2`      |                               |
|r.TranslucencyVolumeBlur			|`0-1`      |                               |
|r.MaterialQualityLevel				|`0-2`		|1 High Quality, 2 Medium, 0 Low|
|r.EmitterSpawnRateScale			|`0.125-1.0`|                               |
|r.ParticleLightQuality				|`0-2`      |                               |


## Subsurface Scattering Quality

| Command |Value      |Effect                        |
|-----------------------------------|-----------|-------------------------------|
|r.SSS.Scale						|`0-1`      |                               |
|r.SSS.SampleSet					|`0-2`      |                               |
|r.SSS.Quality						|`-1 - 1`   |0 Low, -1 Medium, 1 High|
|r.SSS.HalfRes						|`1-0`      |                               |


## Foliage Quality
| Command |Value     |Effect                        |
|-----------------------|-----------|------------------------------|
|foliage.DensityScale	|`0-1`		|0 Stops rendering grass|
|grass.DensityScale		|`0-1`		|0 Stops rendering grass|

## General Commands


| Command |Value          	|Effect                       			    |
|-----------------------|-------------------|-------------------------------------------|
|open					|ip or level name	|Connect to given ip or opens a level		|
|streammap				|level name			|Loads typed level without unloading current level|
|fov					|`0-360`			|Field of View								|
|enablecheats			|`0-1`				|Cheats										|
|ToggleDebugCamera		|					|Enable debug camera						|
|teleport				|					|Teleports character to where camera looks	|
|summon					|bpname_c			|Summons the typed blueprint				|



## ShowDebug TYPE Command

Usage: ShowDebug NONE or ShowDebug CAMERA

| TYPE   | Effect                              |
| ------ | ----------------------------------- |
| NONE   | Shows basic informaton              |
| CAMERA | Current camera position, fov, angle |
| RESET  | Disables the command                |



## Demo Playback
!!! note
	Only works when map is opened using `open` command. Otherwise loads into GlobalPersistentLevel. ***Works but mostly broken.***

| Command | Value | Description |
| ------- | ----- | ----------- |
|demo.AsyncLoadWorld |  |  |
|demo.CheckpointSaveMaxMSPerFrameOverride |  |  |
|demo.CheckpointUploadDelayInSeconds |  |  |
|demo.ClientRecordAsyncEndOfFrame |  |  |
|demo.CullDistanceOverride |  |  |
|demo.EnableCheckpoints |  |  |
|demo.FastForwardDestroyTearOffActors |  |  |
|demo.FastForwardSkipRepNotifies |  |  |
|demo.ForceDisableAsyncPackageMapLoading |  |  |
|demo.ForceFailure |  |  |
|demo.GotoTimeInSeconds |  |  |
|demo.LoadCheckpointGarbageCollect |  |  |
|demo.Loop |  | Loop playing demo |
|demo.MinRecordHz |  |  |
|demo.QueueCheckpointChannels |  |  |
|demo.RecordHz |  |  |
|demo.RecordHzWhenNotRelevant |  |  |
|demo.SkipTime |  |  |
|demo.TimeDilation |  | Slow down currently playing demo |
|demo.UseAdaptiveReplayUpdateFrequency |  |  |
|demo.UseNetRelevancy |  |  |
|DEMOPAUSE |  | Pause currently playing demo |
|DEMOPLAY |  | Start playing demo |
|DEMOREC |  | Start recording demo |
|DEMOSCRUB |  |  |
|DEMOSPEED |  | Demo playback speed |
|DEMOSTOP |  | Stops currently playing demo |
|r.DemosaicVposOffset |  |  |
