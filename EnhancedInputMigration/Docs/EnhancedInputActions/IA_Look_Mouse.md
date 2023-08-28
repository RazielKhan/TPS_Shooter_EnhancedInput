# `IA_Look_Mouse`

## Add Player EnhancedInputAction for `IA_Look_Mouse`
#### Mouse Look movement

>`BP_PlayerCharacterBase` -> `Event Graph` -> `Aiming Input` -> `Look up/down -mouse`
>
>Replace the following `Input Mappings`:
>
>`InputAxis LookUpMouse` -> `EnhancedInputAction IA_Look_Mouse`
>
>![image](./../../Images/EnhancedInput_Aiming_01.png)
>
>`InputAxis Turn` -> `EnhancedInputAction IA_Look_Mouse`
>
>![image](./../../Images/EnhancedInput_Aiming_02.png)

Next, we must search all and replace legacy `InputAction` references with the new `EnhancedInput` actions.

>| Remove Legacy `InputAction` | Replace with `EnhancedAction` | Return Variable Out |
>| --- | --- | --- |
>| `Get Turn` | `Get IA_Look_Mouse` | `X` |
>| `Get LookUpMouse` | `Get IA_Look_Mouse` | `Y` |
>| `Get LookUp` | `Get IA_Look_Mouse` | `Y` |
>
> Example of one replacement:
>
>![image](./../../Images/EnhancedInput_Aiming_07.png)
