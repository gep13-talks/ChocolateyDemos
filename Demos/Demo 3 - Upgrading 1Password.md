## Upgrading 1Password

1. Go to c:\vagrant\resources\installers folder
1. Right click on the oldest 1Password Installer
1. Select Create Chocolatey Package w/out GUI...
1. Show the generated output
1. Copy the nupkg into the c:\vagrant\packages folder
1. Open add/remove programs
1. Show that 1password is not installed
1. Run choco install 1password
1. Show it appear in add/remove programs
1. Back to the installers folder
1. Right click on the newest 1password installer
1. Select Create Chocolate Package
1. Show the Package Builder UI
1. Change the output folder to something other
1. Click generate
1. Take the generated nupkg and put it into the c:\vagrant \packages folder
1. Run choco upgrage 1Password
1. Talk through the output

