# Roblox-Module-Framework

This is a simple framework used for creating more intuitively organized Roblox projects.

* Allows us to write all of our logic inside of Module Scripts.
    * This enables us to easily share code, without having to extract it, create another module script, add the logic, and then require it.
* Organize our server-side logic as "Services" and our client-side logic as "Controllers."

## Usage

The easiest way to use this, would be to download the `Module-Framework.rbxl` file from this repo or the releases page, then import that file into Roblox.

This framework consists of a single Module Script, Script, & Local Script.
* ModuleLoader: is a module script stored inside of the Replicated Storage. This will be required by the server & client, which it will then require all of our Service and Controller modules.
* Loader(s): is a script or local script stored inside of the Server Script Service and the Starter Player Scripts. This script will require our ModuleLoader module from the Replicated Storage, which will then handle requiring all of our other modules.

Once you have your scripts setup, you want to create a Folder called "Services" inside of the Server Script Service and a Folder called "Controllers" inside of the Starter Player Scripts. You will store all of your Module Scripts inside of these folders.

## Example

Inside of the `example` directory of this repo, you will find a brief example of how I use this framework. It includes the framework setup, as well as two Services & Controllers. Keep in mind that these Services & Controllers do not actually function as these were extracted from my [Super Simple Obby](https://www.roblox.com/games/13626754977/Super-Simple-Obby) project.

Along with showing how the framework is used, it also displays how I organize my logic inside of the Module Scripts by using the Local & Shared tables.

## Resources

* [Article going more in-depth, along with a tutorial](https://monzter.dev/lessons/the-module-framework/)
* [Video Tutorial](https://www.youtube.com/@MonzterDEV) (Coming soon)
