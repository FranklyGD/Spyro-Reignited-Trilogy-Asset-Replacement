## Ladders

Collision object requires `Wall.Climb` component tag combined with `ClimbTriggerSpawner`. Position and Rotate so arrow looks at your climbable object.

## Surface Types

| Component Tag               | Function                                                     |
| --------------------------- | ------------------------------------------------------------ |
| TerrainType.IceSkate        | Spyro 2 Ice Skating                                          |
| TerrainType.IceSkate.Spyro3 | Spyro 3 Ice Skating                                          |
| Wall.Climb                  | Makes surface wall climbable, use with `ClimbTriggerSpawner` |
| TerrainType.SlideDown       | Ramp Slide Spyro 3                                           |
| TerrainType.SlideOff        | Sliding down from a platform rotating                        |
| TerrainType.SlideOff.Belly  | Sliding down from a platform on his belly                    |
| Crash                       | Crashes Skateboard? Unsure                                   |
| LaunchRamp (Actor Tag)      |                                                              |
| LaunchRamp_302_001          |                                                              |
| LaunchRamp_302_004          |                                                              |

## Gameplay Effects

| Name                                           | Observed Effect                                              |
| ---------------------------------------------- | ------------------------------------------------------------ |
| GE_BasicDamage                                 | Decrease One Hitpoint                                        |
| GE_BasicHeal                                   | Increase One Hitpoint                                        |
| GE_HitReact_Standard                           | Lose Control                                                 |
| GE_Invincibility                               | unknown                                                      |
| GE_LevelTransition                             | unknown                                                      |
| GE_OneHitKill                                  | Die from one hit                                             |
| GE_Cutscene                                    | unknown                                                      |
| GE_SpyroFlightLevel                            |                                                              |
| GE_CameraDisableUpdateVisibility.uasset        |                                                              |
| GE_CenterCamera.uasset                         |                                                              |
| GE_CenterCameraHold.uasset                     |                                                              |
| GE_DamageWaterImpairedInput.uasset             |                                                              |
| GE_ImmuneFireFront.uasset                      |                                                              |
| GE_NoOrientRotationToMovement.uasset           |                                                              |
| GE_Spyro2IceSkating.uasset                     | Auto walks forward, can charge, might need an ice surface to play the animation forcing skating animation works |
| GE_SpyroChargeGravity.uasset                   |                                                              |
| GE_SpyroCharge_DisableFly.uasset               |                                                              |
| GE_SpyroClimbDisableJumpInput.uasset           |                                                              |
| GE_SpyroClimbing.uasset                        | Doesn't climb, really slow glide, walk, charging             |
| GE_SpyroClimbingDetach.uasset                  |                                                              |
| GE_SpyroCrashAirDisableInput.uasset            |                                                              |
| GE_SpyroCrashing.uasset                        |                                                              |
| GE_SpyroCustomProjectile.uasset                |                                                              |
| GE_SpyroDamageBossKnockUp.uasset               | Can't jump and charge, nothing happens                       |
| GE_SpyroDamageLavaKnockUp.uasset               |                                                              |
| GE_SpyroDamageRegionCharge.uasset              |                                                              |
| GE_SpyroDamageRegionSuperCharge.uasset         |                                                              |
| GE_SpyroDisableAllInput.uasset                 |                                                              |
| GE_SpyroDisableAllInput_Invuln.uasset          |                                                              |
| GE_SpyroDisableChargeCrashInterval.uasset      |                                                              |
| GE_SpyroDisableChargeFromRoll.uasset           |                                                              |
| GE_SpyroDisableFaceBottom.uasset               |                                                              |
| GE_SpyroDisableFlyingModes.uasset              |                                                              |
| GE_SpyroDisableFreeLook.uasset                 |                                                              |
| GE_SpyroDisableFreeLookAbilityOnly.uasset      |                                                              |
| GE_SpyroDisableGliding.uasset                  | Disables gliding                                             |
| GE_SpyroDisableGravity.uasset                  |                                                              |
| GE_SpyroDisableLoot.uasset                     |                                                              |
| GE_SpyroFlightCamAllowControl.uasset           |                                                              |
| GE_SpyroFlightCamVertRotation.uasset           |                                                              |
| GE_SpyroFlightDisableLoops.uasset              |                                                              |
| GE_SpyroFlightLevel.uasset                     |                                                              |
| GE_SpyroFlightSpeedControl.uasset              |                                                              |
| GE_SpyroFlying.uasset                          |                                                              |
| GE_SpyroFlyingFlapping.uasset                  |                                                              |
| GE_SpyroFlyLoop.uasset                         |                                                              |
| GE_SpyroFlySpeedBoost.uasset                   |                                                              |
| GE_SpyroFly_DisableCharge.uasset               |                                                              |
| GE_SpyroGliding.uasset                         |                                                              |
| GE_SpyroHeadBash.uasset                        |                                                              |
| GE_SpyroHeadBashLand.uasset                    |                                                              |
| GE_SpyroHover.uasset                           |                                                              |
| GE_SpyroHoverDisableFlight.uasset              |                                                              |
| GE_SpyroHoverTank.uasset                       |                                                              |
| GE_SpyroHoverTankBoss.uasset                   |                                                              |
| GE_SpyroHoverTankBoss_KBM.uasset               |                                                              |
| GE_SpyroIceBreathEnabled.uasset                | Ice spikes powerup                                           |
| GE_SpyroIceFireEnabled.uasset                  | Ice breath - Frozen Altars                                   |
| GE_SpyroIceSkating.uasset                      |                                                              |
| GE_SpyroJumpGracePeriod.uasset                 |                                                              |
| GE_SpyroJumpMushroom.uasset                    |                                                              |
| GE_SpyroJumpNoGravity.uasset                   |                                                              |
| GE_SpyroLedgeHover.uasset                      |                                                              |
| GE_SpyroMantaRay.uasset                        |                                                              |
| GE_SpyroMantaRayBoost_Spyro3.uasset            |                                                              |
| GE_SpyroMantaRayMovement_Spyro3.uasset         |                                                              |
| GE_SpyroMantaRay_Spyro3.uasset                 |                                                              |
| GE_SpyroMicroGravity.uasset                    |                                                              |
| GE_SpyroRageFireEnabled.uasset                 | Fairy Kiss breath                                            |
| GE_SpyroSaucerRide.uasset                      |                                                              |
| GE_SpyroSaucerRideBoss.uasset                  |                                                              |
| GE_SpyroSideRolling.uasset                     |                                                              |
| GE_SpyroSlideDown.uasset                       |                                                              |
| GE_SpyroSlideDownFall.uasset                   | Sliding down on ice                                          |
| GE_SpyroSlidingOff.uasset                      |                                                              |
| GE_SpyroSpeedControl.uasset                    |                                                              |
| GE_SpyroSpitItem.uasset                        |                                                              |
| GE_SpyroSubmarineRide.uasset                   |                                                              |
| GE_SpyroSuperChargeAltForceOn.uasset           |                                                              |
| GE_SpyroSuperChargeEnableAlt.uasset            |                                                              |
| GE_SpyroSuperChargeEnabled.uasset              | Enable supercharge (3 stage)                                 |
| GE_SpyroSuperChargeForceOn.uasset              |                                                              |
| GE_SpyroSuperChargeGate.uasset                 |                                                              |
| GE_SpyroSuperChargeJumpAssistEnabled.uasset    |                                                              |
| GE_SpyroSuperChargeRampFail.uasset             |                                                              |
| GE_SpyroSuperChargeStageAlt.uasset             |                                                              |
| GE_SpyroSuperChargeStageOne.uasset             |                                                              |
| GE_SpyroSuperChargeStageThree.uasset           |                                                              |
| GE_SpyroSuperChargeStageTwo.uasset             |                                                              |
| GE_SpyroSuperCharging.uasset                   | Only effects show, charge speed same                         |
| GE_SpyroSuperFireEnabled.uasset                | Superflame                                                   |
| GE_SpyroSuperFlyEnabled.uasset                 | Free Flight                                                  |
| GE_SpyroSuperJumping.uasset                    | Increases jump height, makes Spyro move forward until jump   |
| GE_SpyroSwimcamCentering.uasset                | Camera used in underwater                                    |
| GE_SpyroSwimFromHeadBash.uasset                |                                                              |
| GE_SpyroSwimmingDiving.uasset                  |                                                              |
| GE_SpyroSwimmingSurface.uasset                 |                                                              |
| GE_SpyroSwimmingUnderwater.uasset              | Puts spyro in underwater state, allows swimming in physics volume, broken camera, use GE_SpyroSwimcamCentering for camera |
| GE_SpyroTempDisableJumpStop.uasset             |                                                              |
| GE_SpyroTurretBoss.uasset                      |                                                              |
| GE_Spyro_DamageTransientBossLevitate.uasset    |                                                              |
| GE_Spyro_DisableInput_SuperJumping.uasset      |                                                              |
| GE_Spyro_Movement_ChargeJumping.uasset         |                                                              |
| GE_Spyro_Movement_Charging.uasset              |                                                              |
| GE_Spyro_Movement_ChargingUnderwater.uasset    |                                                              |
| GE_Spyro_Movement_Jump.uasset                  |                                                              |
| GE_Spyro_Movement_SuperChargeJumping.uasset    |                                                              |
| GE_Spyro_Movement_SuperChargeJumpingMax.uasset |                                                              |
| GE_Spyro_Movement_SuperCharging_Alt.uasset     |                                                              |
| GE_Spyro_Movement_SuperCharging_S0.uasset      |                                                              |
| GE_Spyro_Movement_SuperCharging_S1.uasset      |                                                              |
| GE_Spyro_Movement_SuperCharging_S2.uasset      |                                                              |
| GE_Spyro_Movement_SuperCharging_S3.uasset      |                                                              |
| GE_Spyro_Movement_SuperJump.uasset             |                                                              |
| GE_Spyro_Movement_SwimmingTunnel.uasset        |                                                              |
| GE_Spyro_Movement_SwimmingTunnel332.uasset     |                                                              |
| GE_Spyro_Movement_SwimmingUnderwater.uasset    |                                                              |
| GE_Spyro_RapidFire.uasset                      | Holding left click does breathing animation continuesly but no fires come out |
| GE_Spyro_RapidFiringState.uasset               |                                                              |
| GE_WhirlwindInteraction.uasset                 |                                                              |

Simple usage for Gameplay Effects

![spawner_blueprint_setup](assets/spawner_blueprint_setup.png)