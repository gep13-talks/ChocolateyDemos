##Installing Chocolatey##

1. Open a command prompt as an Administrator
1. Open the chocolatey.org home page in your browser of choice
1. Copy the text from the home page, or take the following
```powershell
@powershell -NoProfile -ExecutionPolicy unrestricted -Command "iex ((new-object net.webclient).DownloadString('http://chocolatey.org/install.ps1'))" && SET PATH=%PATH%;%systemdrive%\chocolatey\bin
```
1. Paste into the command prompt you opened earlier
1. Click Enter
1. Job done!
1. Open File Explorer
1. Navigate to C:\Chocolatey
1. Explain about the various folders
1. Show environment variables have also been created
1. Open a Powershell window as an administrator and run the following:

```powershell
chocolatey help
```