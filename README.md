# TPS_Shooter_EnhancedInput
Update 08/28/2023: Fixed `InputAction` mapping for movement to fix bug that would keep the player in a run animation state when done moving.

Update 09/04/2023: Created new `TriggerUpdateLook` event to trigger the camera pitch/yaw per tick. IA_Look_Mouse isn't called per tick as the default input action was, and resulted in bugs where the player character wouldn't fully rotate towards the aim point if the mouse wasn't actively moving (creating trigger events).

Enhanced Input migration documentation and inputs for Third Person Shooter Kit for UE5. https://www.unrealengine.com/marketplace/en-US/product/third-person-shooter-kit?

The work I've done for the [TPS-K Enhanced Input Tracker](./EnhancedInputMigration/Docs/EnhancedInputTracker.md) documents the steps to migrate the TPS-K from *Legacy* `InputAction` to `EnhancedInput`. When migrating, please note that there are some initial steps documented that need to occur before implementing each of the `IA_<action_name>` Input Events.

Please see [TPS-K Enhanced Input Tracker](./EnhancedInputMigration/Docs/EnhancedInputTracker.md) for details on how to start migrating your TPS-K UE5 project.

>Please note that the UE5 Blueprint files are located here: [./EnhancedInputMigration/EnhancedInput/](./EnhancedInputMigration/EnhancedInput/) These can be migrated into your current project. For my setup, I put them in:
>
>- `/Content/ThirdPersonKit/Blueprints/EnhancedInput/...`
>- `/Content/ThirdPersonKit/Blueprints/EnhancedInput/Actions/...`
>- `/Content/ThirdPersonKit/Blueprints/EnhancedInput/Configs/...`
>- `/Content/ThirdPersonKit/Blueprints/EnhancedInput/Mappings/...`
>- `/Content/ThirdPersonKit/Blueprints/EnhancedInput/MiscClasses/...`
>- `/Content/ThirdPersonKit/Blueprints/EnhancedInput/Settings/...`

*Additional note, some user input keys are not yet hooked up from the original project. I do not cover these in this migration document yet.*