Cake
====

This extension contains a custom build task that runs Cake build scripts for you.

Cake (C# Make) is a cross platform build automation system with a C# DSL to do things like compiling code, copy files/folders, running unit tests, compress files and build NuGet packages.

Run Cake scripts easily
-----------------------

The Cake VSO build tasks makes it easy to run a Cake script directly without having to invoke PowerShell or other commands line scripts. This makes it easy even for team members not familiar with Cake to add or adjust parameters passed to your build scripts.

How to use the build task
-------------------------

After installing this extension, a new task will become available called "Cake Task" when you add a new build step for a build definition.

![Add Cake Task](Images/addtasks.png)

By default, the Cake build step (when added to a build) will try to run the `build.cake` build script (found in the root of your repository) with the target `Default`. If you wish to run another build script or build target you can change this in the build step settings.

![Configure Custom Build Step](Images/configurebuildstep.png)

At the moment, only Windows build agents are supported, but we expect to add support for other build agents soon.

Learn more
----------

For more information about Cake, please see the [Cake website](http://cakebuild.net) or the Cake [source code repository](https://github.com/cake-build/cake).
