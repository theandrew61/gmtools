# gmtools
Access gmad and gmpublish within Garry's Mod!

# Installation
Installing gmtools to Garry's Mod is easy.
Steps:
1. Download the latest release for your platform.
2. Extract the *.zip* to ```garrysmod/lua/bin```. The zip contains:
  - *gmcl_gmtools_win32.dll* - the library
  - *gmad.exe* - gmad
  - *gmpublish.exe* - gmpublish
3. In  ```garrysmod/addons```, either move the *.gma* to there, or clone the mod's repo in there.

# API
### ```gmtools.create_gma(inputFolder, outputGMA)```
Description:
- Creates a *.gma* file based on the inputFolder.

Parameters:
- inputFolder (required): the path to the mod you want to create
- outputFolder (optional): the path to the *.gma*

Example:
```gmtools.gmad_create("C:\Users\andrew\Desktop\mod", "C:\Users\andrew\Desktop\mod.gma")```

# Credits
Inspired by g-ace-io
