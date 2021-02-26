# Modules
What are modules and what it does? Well you can read it here!

## What is a module?
A module is a piece of code that can be loaded and unloaded at runtime, giving or removing a feature to OpenBlocks.

So, there are 5 Important Types of modules in OpenBlocks: (we'll add more soon)
 - `PROJECT_MANAGER`: Manages where the projects are located, are written, and are read.
 - `PROJECT_PARSER`: Parses files (that you can get from `PROJECT_MANAGER`) into a Layout, and Code.
 - `PROJECT_GUI_LAYOUT`: Displays a View that allow the user to visualize / edit the layout.
 - `PROJECT_GUI_CODE`: Displays a View that allow the user to visualize / edit the Code.
 - `PROJECT_COMPILER`: Compiles the Layout and Code into a single ready-to-install APK file.

OpenBlocks need atleast one module of each type for it to work as these modules are important.

So, yeah, after reading this, OpenBlocks is just a simple structure, where the features came from modules.

## What's cool with it?
You see, Most apps are not dynamic, they just works on how they were built, giving the user have no control of the features / issues of the app. With this modular approach, users can create features as they like, Do what they want!
