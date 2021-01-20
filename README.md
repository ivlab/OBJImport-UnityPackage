# OBJImport

OBJImport library from Dummiesman, originally sourced from the [Unity Asset
Store](https://assetstore.unity.com/packages/tools/modeling/runtime-obj-importer-49547)

## Updating/Creating a new package

This package was generated from a [NuGet](https://www.nuget.org/) package.
Follow the instructions below to update this package or make a new Unity package
from a NuGet package.


## Setup

1. Open a new blank Unity project
  - The project will not contain anything, this is useful solely for creating
    the package
2. Download the latest NuGet Unity Asset .unitypackage file from the [Releases Page of
NuGetForUnity](https://github.com/GlitchEnzo/NuGetForUnity/releases/)
  - At the time of this writing, latest version was v2.0.1
3. Import the asset into Unity by dragging and dropping, or *Assets > Import New
   Asset...*, and import everything from the asset
  - A new menu, *NuGet*, should appear on the top bar for Unity


## Download a NuGet Package

1. In Unity, go to *NuGet > Manage NuGet Packages*
2. Search for your package
3. Click "Install" on the package you want - this will import it into a folder
   in your project *Assets / Packages / YourPackage*


## Set up a new Unity Package

1. If making a new package, create a new GitHub repository for your package in
the [IVLab GitHub](https://github.umn.edu/ivlab-cs)
  - Name it `YourPackage-UnityPackage` (replace "YourPackage" with the actual
    package name)
  - Add the word "NuGet" somewhere in the repo description
2. Clone the repo into the *Packages* folder in your blank Unity project
  - Not *Assets / Packages*, just *Packages*!
3. Copy this README.md into that repo and change the title/description at the top
4. Make a new commit "Initial commit" with the README


## Add contents from NuGet package

1. Make a new folder *Runtime* inside the repo *Packages / YourPackage-UnityPackage*
2. Copy the NuGet package (downloaded earlier) from *Assets / Packages* into
   *Packages / YourPackage-UnityPackage / Runtime*
3. Create a new file *package.json* inside *Packages / YourPackage-UnityPackage*
   and copy the following contents into it, replacing the fields as you see fit
   (ideally the version should match the NuGet package and the description
   should contain the word "NuGet"):

```
{
    "name": "edu.umn.cs.ivlab.yourpackage",
    "displayName": "YourPackage",
    "version": "0.0.1",
    "unity": "2020.1",
    "description": "Your description goes here",
    "dependencies": {}
}
```

4. Commit and push these changes to your GitHub repository, and optionally make
   a tag for this version release
