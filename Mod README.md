# gmtools (Garry's Mod mod)
This file explains the gmtools mod, not the gmtools API.

# Usage
Usage of the mod is very similar to the gmtools' API. Open the console and have fun!

**Note: all paths must be wrapped in double quotes (")**, otherwise errors will arise.

### ```gmad_create inputFolder, outputGMA```
Description:
- Creates a *.gma* file based on the inputFolder.

Parameters:
- inputFolder (required): the path to the mod you want to create
- outputGMA (optional): the path to the *.gma*, **note**: the *.gma* extenesion will be added by gmad if it isn't there

Returns:
- string: whatever gmad returns

Example:
```gmad_create "C:\Users\andrew\Desktop\mod" "C:\Users\andrew\Desktop\mod.gma"```

### ```gmad_extract inputGMA outputFolder```
Description:
- Extracts the inputGMA.

Parameters:
- inputGMA (required): the path to the *.gma* you want to create
- outputFolder (optional): the path where the *.gma* will be extracted

Returns:
- string: whatever gmad returns

Example:
```gmad_extract "C:\Users\andrew\Desktop\mod.gma" "C:\Users\andrew\Desktop\mod"```

### ```gmpublish_list```
Description:
- Lists all the mods you have uploaded to the Garry's Mod Workshop.

Parameters:
- none

Returns:
- string: whatever gmpublish returns

Example:
```gmpublish_list```
