# gmtools
Access gmad and gmpublish within Garry's Mod!

# Table of Contents
- [Installation](#table-of-contents)
- [API](#api)
- [Building](#building)
- [Known issues](#known-issues)
- [Credits](#credits)

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
### ```gmtools.gmad_create(inputFolder, outputGMA)```
Description:
- Creates a *.gma* file based on the inputFolder.

Parameters:
- inputFolder (required): the path to the mod you want to create
- outputGMA (optional): the path to the *.gma*, **note**: the *.gma* extenesion will be added by gmad if it isn't there

Returns:
- string: whatever gmad returns

Example:
```gmtools.gmad_create("C:\Users\andrew\Desktop\mod", "C:\Users\andrew\Desktop\mod.gma")```

### ```gmtools.gmad_extract(inputGMA, outputFolder)```
Description:
- Extracts the inputGMA.

Parameters:
- inputGMA (required): the path to the *.gma* you want to create
- outputFolder (optional): the path where the *.gma* will be extracted

Returns:
- string: whatever gmad returns

Example:
```gmtools.gmad_extract("C:\Users\andrew\Desktop\mod.gma", "C:\Users\andrew\Desktop\mod")```

### ```gmtools.gmpublish_list()```
Description:
- Lists all the mods you have uploaded to the Garry's Mod Workshop.

Parameters:
- none

Returns:
- string: whatever gmpublish returns

Example:
```print(gmtools.gmpublish_list())```

# Building
## Windows
You will need:
- premake4 (included)
- Visual Studio 2010 or newer (I used VS 2015)
- Garry's Mod

Steps:
1. Clone the repo.
2. Run *CreateSln.bat*. This will generate a Visual Studio solution.
3. Open the solution and build it.
## macOS & Linux
none yet

# Known issues
- When listing the contents of a mod with numerous files inside, the printing is truncated - this is an issue with char arrays
![](http://i.imgur.com/RigKwyd.jpg)

# Credits
Inspired by g-ace-io
