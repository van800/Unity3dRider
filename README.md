# Unity3dRider

## How to use:
1. Open Unity
2. Menu `Edit` -> `Preferences` -> `External Tools`
3. `External Script Editor` -> `Browse` -> Select `Rider.exe` / `.lnk`, `rider.sh` or `Rider.app` depending on the OS
4. Put the folder `Assets/Plugins/Editor/` from this repository into `Assets/Plugins/` in your project.
5. Double clicking a file or error message in Unity should open Rider and navigate to the corresponding file and line.

The plugin should work on Windows, Linux and macOS.

## Common problems solved by this plugin
1. Basic Open Solution and Navigate to file and line
2. RIDER-1261 Symbols are not resolved across projects in a single solution (i.e. Unity Editor scripts do not see symbols in main project)
3. 'Go To Declaration' problem. Details here https://rider-support.jetbrains.com/hc/en-us/community/posts/207243685-Unity3D-support
4. RIDER-573 System.Linq can not be found in a new Unity project
5. Simple Debugging UnityEditor is implemented within the plugin, but better debugging support is planned in Rider itself- follow https://youtrack.jetbrains.com/issue/RIDER-485
6. LangVersion is set to 5.0, which prevents Rider to suggest C# 6 language improvements
