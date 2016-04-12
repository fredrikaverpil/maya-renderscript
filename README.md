# maya-renderscript

Combine multiple *.mel and/or *.py scripts to be used on Maya commandline rendering.

### Installation

Place `maya-renderscript.mel` script in your `MAYA_SCRIPT_PATH`.
 
### Usage

Use the MEL function when commandline rendering and feed it any number of scripts.

Example:
```
Render.exe -preRender "RenderScriptConsolidator({\"C:/preRender.mel\", \"C:/preRender.py\", \"C:/preRender2.py\"})" C:/MayaProject/scenes/MyScene.ma
```
### Please note

* Any existing MEL in the Maya scene file's render globals/render options is overridden by this consolidation.
* Has been tested with Maya 2014, 2015, 2016 on Windows and Linux.

