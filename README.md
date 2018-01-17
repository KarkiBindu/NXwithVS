# NXwithVS
Configration for NX with Visal Studio

I am using NX 11 with Visual Studio 2015. After Installing Nx and Visual studio:

    copy vcprojects from C:\Program Files\Siemens\NX 11.0\UGOPEN\vs_files\VC to C:\Program Files (x86)\Microsoft Visual Studio 12.0\VC\VCWizards
    and copy VCWizards to C:\Program Files (x86)\Microsoft Visual Studio 12.0\VC\vcprojects

Then create a new ClassLibrary Project in Visual Studio and Give Refernece to the Reqired libararies of NX like:

    NXOpen
    NXOpen.UF
    NXOpenUI
    NXOpen.Utilities

These all files are located in C:\Program Files\Siemens\NX 11.0\NXBIN\managed

Then build the project

A .dll file with project name is created inside the bin folder of the project directory which is used execute the code in NX


To use these libraries on visual studio 
* `using NXOpen`  
* `using NXOpen.UF`.... is used
