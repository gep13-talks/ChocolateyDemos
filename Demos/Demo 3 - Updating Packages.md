##Updating Packages##

1. Open a PowerShell as an Administrator
1. Type the following command:

```powershell
cinst chocolateygui -version 0.11.0
```

1. Press enter
1. This will install an earlier version of the GUI package
1. Back to the PowerShell Windows, type the following:

```powershell
cver chocolateygui
```

1. Show how there is a newer version ready to be installed
1. Type the following:

```powershell
cup chocolateygui
```

1. Press enter
1. Show latest version is installed
1. Open File Explorer
1. Navigate to C:\Chocolatey\lib
1. Show two entries now for ChocolateyGUI
1. Back at PowerShell Window type:

```powershell
cuninst chocolateygui
```

1. Show the Chocolatey\lib folder and show that only the latest version has been removed from the lib folder, but that both packages have been removed from system.
1. Back at the PowerShell window type the following:

```powershell
cup all
```
1. Press enter
1. Explain it will update all installed packages
1. Back at the PowerShell window type the following:

```powershell
cup
```

1. Press enter
1. Explain how this will update chocolatey itself