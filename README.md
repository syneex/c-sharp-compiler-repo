# Purpose...
... of this repository is to play around with the process of C# compiling, learning all the steps (including CLR, IL and JIT) as well as having a reference for future situations.

## Tutorials
### How to get Intermediate Language Code from C# Compiler
Needed Resources:
- Visual Studio with any C# version installed
- A hello world app

First, build the application so that the .dll + .exe files are generated (for c# they are located in {PROJECTLOCATION}\bin\{projectConfiguration}\{TargetFramework} -> possibility: C:\Users\User\source\repos\HelloWorld\bin\Debug\net6.0). Now open Visual Studio with the "hello world" app, get the developer command prompt for visual studio and navigate to the dll files in the path above. Now type in "ILDASM". A window will pop up - there select "File", "Open" and select the .dll file of your application. Now everything is loaded into the ILDASM and you can check out the intermediate language code.
