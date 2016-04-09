##Creating your own Chocolatey Package##

1. Open a PowerShell Windows as an Administrator
1. Type the following:

```powershell
cinst warmup
```

1. Press enter
1. Back at the command line, run the following commands:

```powershell
warmup addTextReplacement __CHOCO_PKG_OWNER_NAME__ "Gary Ewan Park"
```

```powershell
warmup addTextReplacement __CHOCO_PKG_OWNER_REPO__ "https://github.com/gep13/ChocolateyPackages"
```

```powershell
warmup addTextReplacement __CHOCO_AUTO_PKG_OWNER_REPO__ "https://github.com/gep13/ChocolateyAutomaticPackages"
```

1. Click Enter
1. Create a folder at the root of your c:\ drive called github, and navigate into it with PowerShell Window
1. Type the following:

````powershell
git clone https://github.com/chocolatey/chocolateytemplates.git
```

1. Press Enter
1. Navigate into the chocolateytemplates\_templates folder in PowerShell window and execute the following commands:

```powershell
warmup addTemplateFolder chocolatey "%cd%\chocolatey"
```

```powershell
warmup addTemplateFolder chocolatey3 "%cd%\chocolatey3"
```

```powershell
warmup addTemplateFolder chocolateyauto "%cd%\chocolateyauto"
```

```powershell
warmup addTemplateFolder chocolateyauto3 "%cd%\chocolateyauto3"
```

1. Now, in PowerShell, navigate to the folder, most likely a git repo, where you want to create the files for your chocolatey package
1. Type the following command:

```powershell
warmup chocolatey fiddler4
```

1. Press Enter
1. This will create the default package for your including the .nuspec file, and the tools\chocolateyInstall.ps1
1. All we need to do now is fill this in.
1. Open the nuspec file and replace with the following:

```powershell
<?xml version="1.0"?>
<package xmlns="http://schemas.microsoft.com/packaging/2010/07/nuspec.xsd">
  <metadata>
    <id>fiddler4</id>
    <title>Fiddler</title>
    <version>4.4.3</version>
    <authors>Telerik</authors>
    <owners>Gary Ewan Park</owners>
    <summary>Fiddler Web Debugging Proxy</summary>
    <description>Fiddler is a Web Debugging Proxy which logs all HTTP(S) traffic between your computer and the Internet. Fiddler allows you to inspect all HTTP(S) traffic, set breakpoints, and "fiddle" with incoming or outgoing data. Fiddler includes a powerful event-based scripting subsystem, and can be extended using any .NET language.

Fiddler is freeware and can debug traffic from virtually any application, including Internet Explorer, Mozilla Firefox, Opera, and thousands more.</description>
    <projectUrl>http://www.fiddler2.com/fiddler2/</projectUrl>
    <tags>fiddler fiddler2 web debugging proxy admin</tags>
    <copyright></copyright>
    <licenseUrl>http://www.fiddler2.com/Fiddler/help/license.asp</licenseUrl>
    <requireLicenseAcceptance>false</requireLicenseAcceptance>
    <iconUrl>https://github.com/gep13/ChocolateyPackages/raw/master/fiddler4/FiddlerLogo.png</iconUrl>
    <releaseNotes></releaseNotes>
  </metadata>
  <files>
    <file src="tools\**" target="tools" />
  </files>
</package>
```

1. Open the chocolateyInstall.ps1 file and replace with the following:

```powershell
$packageName = 'fiddler4'
$installerType = 'EXE'
$url = 'http://www.getfiddler.com/dl/Fiddler4BetaSetup.exe'
$url64 = $url
$silentArgs = '/S'
$validExitCodes = @(0,1)

Install-ChocolateyPackage "$packageName" "$installerType" "$silentArgs" "$url" "$url64"  -validExitCodes $validExitCodes
```
1. Open a PowerShell Window to where you created the above, and then simply run the following:

```powershell
cpack
```

1. And the chocolatey package will get created.
1. job done!