# Dusty Utilities
Small Unity package to aid in basic scripting.
Created for Dusty Studios in game development

### Save script
- Helper script to save given data
- Support for any class
- Saves to JSON under given file name

## Dusty utils import overview
Add "using static DustyUtils.Utils" or "using static DustyUtils.SaveUtils" to use available functions

### Utils
- GetAllComponentsFromGameObjectChildren<T>(Transform parent) - returns all components from all children in a parent object
- GetRandomArrayElement<T>(Array array) / GetRandomListElement<T>(List<T> list) - returns a random "element" or "value" from an array or list
- CheckGetComponent<T>(Gameobject obj) - returns component from gameObject and logs a warning if a component cannot be found
- GetAngleFromDirection(float directionX, float directionY) - returns Z angle from normalized direction

### Save Utils
- SaveData<T>(T data, string fileName) - saves data as a file name to JSON. (Directory is the persistent data path)
- GetData<T>(string fileName) - retrieves data given a file name, if there is no file, it will return the default of the class
- DeleteData<T>(string fileName) - deletes data given a file name
