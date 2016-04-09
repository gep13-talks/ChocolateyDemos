##Installing Packages##

1. Open a PowerShell as an Administrator
1. Type the following command:

```powershell
cinst chocolateygui
```

1. Press enter
1. Show dependencies being installed
1. Open File Explorer
1. Browse to C:\Chocolatey\lib
1. Show new packages in this folder
1. Go into each package and show the nupkg file, and the difference between packages that include the msi, and others that don't
1. Show the new entry in Add/Remove Programs
1. Go back to the command window and type the following:

```powershell
cuninst chocolateygui
```

1. Refresh Programs list, show it is gone
1. Show C:\Chocolatey\lib folder, and show the removal of package, but that the dependent package is still there