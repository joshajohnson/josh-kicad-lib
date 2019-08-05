# josh-kicad-lib
KiCad library for all of my projects

## To Use
Create a new directory  

Initialise git  
```git init```  

Create library submodule  
``` git submodule add https://github.com/joshajohnson/josh-kicad-lib.git```  

Create a hardware directory, and copy the template folder into hardware folder  

Rename template files as required  

Ready to design your next board!

### Folder Structure
This should result in a folder structure which looks like the below. If your KiCad project is not two levels below this library, things will not work properly.

``` 
kicad-project-git
|- .git
|
|- .gitmodules
|- hardware
|  |- version
|     |- fp-info-cache
|     |- fp-lib-table
|     |- sim-lib-table
|     |- <project>.kicad_pcb
|     |- ...
|
|- josh-kicad-lib
|  |- lib files
|
|- README.md 
```

### Addition of new libraries / 3d models
Ensure all paths use the below text at the start of the path, as this keeps everything relative and ensures that it will work across different locations and computers. 

``` ${KIPRJMOD}/../../josh-kicad-lib/...```