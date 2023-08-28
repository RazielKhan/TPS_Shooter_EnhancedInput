# TPS_Shooter_EnhancedInput

Enhanced Input migration documentation and inputs for Third Person Shooter Kit for UE5. https://www.unrealengine.com/marketplace/en-US/product/third-person-shooter-kit?

The work I've done for the [TPS-K Enhanced Input Tracker](./EnhancedInputMigration/Docs/EnhancedInputTracker.md) documents the steps to migrate the TPS-K from *Legacy* `InputAction` to `EnhancedInput`. When migrating, please note that there are some initial steps documented that need to occur before implementing each of the `IA_<action_name>` Input Events.

Please see [TPS-K Enhanced Input Tracker](./EnhancedInputMigration/Docs/EnhancedInputTracker.md) for details on how to start migrating your TPS-K UE5 project.

>Please note that the UE5 Blueprint files are located here: [./EnhancedInputMigration/EnhancedInput/](./EnhancedInputMigration/EnhancedInput/) These can be migrated into your current project. For my setup, I put them in:
>
>- `/Content/ThirdPersonKit/Blueprints/...`
>- `/Content/ThirdPersonKit/Blueprints/Actions/...`
>- `/Content/ThirdPersonKit/Blueprints/Configs/...`
>- `/Content/ThirdPersonKit/Blueprints/Mappings/...`
>- `/Content/ThirdPersonKit/Blueprints/MiscClasses/...`
>- `/Content/ThirdPersonKit/Blueprints/Settings/...`

*Additional note, some user input keys are not yet hooked up from the original project. I do not cover these in this migration document yet.*