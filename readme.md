# HSI RBX Github Lua Format

An method of storing RBX objects within Github.

Please note that this guide requires some knowledge into the Roblox Lua Engine. As this guide will not cover classNames are and the different properties of them.

## Posible questions:

### Why?

Github currently only stores files like txt, js, html and css files, It has no way of storing RBXL Objects, thus this format was created and is currently assigned to no project.

Note: This may be moved to the HSICore/Reactor project when ready. Although the license will still not be there.

### Why no license?

I want this to be used in any project with RBX objects. Although would be nice if they included attribution.

### May I use this in my Github Repo?

Yes! There are no restrictions to using this! Hence no license, however it would be nice if included attribution to this repo. Although is not required.

## File format:

### Instances:

[This is NOT a guide to instances. This is how instances are stored with in this format.]

#### Naming scheme:

Instances are folders that named with their respective Name and ClassName organized like this:

Name.ClassName

An example of this name would be:

HSICore.Frame

#### Contents:

An instance contains the following [In this format.]:

Other instances, script.lua [If the object is a script] and properties.json

Other instances is self-explanatory.

script.lua contains the script of the instance if the is a Script, LocalScript, ModuleScript or CoreScript.

properties.json contains a list of key-value pairs that relate to the properties of the instance's ClassName. properties.json ***must*** contain the Name and ClassName of the instance. Do not use all of the values, only ones that are shown on the 'Properties Window' of RBX Studio OR is [referenced by a script](https://github.com/ProjectHSI/RBLX-Lua-Format/blob/master/RBAS.Script/script.lua). the **ONLY** exception to this is if it's an instance that can defined using regular files or folders, an example of which is 'instance.RobloxLocked'