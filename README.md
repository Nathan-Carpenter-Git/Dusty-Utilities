# Dusty Utilities
Small Unity package to aid in basic scripting.
Created for Dusty Studios in game development

## Includes
### Customizable movement scripts
- Support for a 2D top-down, physics, and transform-based platformer
- Support for a 3D transform and physics-based game.

### Ground detection script
- Supports 3D and 2D detection for player jumping
- Can use raycast or trigger collision detection
- Ability to add a layer mask

### Save script
- Helper script to save given data
- Support for any class
- Saves to JSON under given file name

## Dusty utils import overview
"using static DustyUtils.Utils" or "using static DustyUtils.SaveUtils" to use available functions

### Utils
- GetRandomArrayElement<T>(Array array) / GetRandomListElement<T>(List<T> list) - returns a random "element" or "value" from an array or list
- CheckGetComponent<T>(Gameobject obj) - returns component from gameObject and logs a warning if a component cannot be found

### Save Utils
- SaveData<T>(T data, string fileName) - saves data as a file name to JSON. (Directory is the persistent data path)
- GetData<T>(string fileName) - retrieves data given a file name, if there is no file, it will return the default of the class
- DeleteData<T>(string fileName) - deletes data given a file name
