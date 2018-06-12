@title[Adding a layer of Chocolate(y)]

## Adding a layer of Chocolate(y)

---
@title[Slides]

## Slides

### https://gep13.me/ChocolateySlides

---

@title[What is Chocolatey?]

## What is Chocolatey?

+++

@title[A Definition...]

### A Definition...

"Chocolatey is a global PowerShell execution engine using the NuGet packaging infrastructure. Think of it as the ultimate automation tool for Windows."

+++

@title[It's Magic!]

![It's Magic](assets/images/magic.gif)

---

@title[Windows Software Ecosystem]

## Windows Software Ecosystem

+++

@title[Traditional Windows]

### Traditionally Windows was designed with Visual Interfaces in mind

+++

@title[Still evident]

### There is no place more evident of that still than in the Windows Software Installer ecosystem

+++

@title[Windows Software Installers]

![Windows Software Installers](assets/images/picard-meme.png)

+++

@title[No Consistency]

### No Consistency

- Over 20 installer formats and thousands of installers in the wild
- Zips and other archive formats
- Software installers are messy
- It's like the wild west

+++

@title[Wild West]

![Wild West](assets/images/clint_eastwood.png)

---

@title[Let's install paint.net]

## Let's install paint.net...

+++

@title[paint.net website]

<!-- .slide: data-transition="none" -->
![Build Step](assets/images/install-paint.net-step-1.png)

+++

@title[Not the paint.net website]

<!-- .slide: data-transition="none" -->
![Build Step](assets/images/install-paint.net-step-2.png)

+++

@title[Google paint.net]

<!-- .slide: data-transition="none" -->
![Build Step](assets/images/install-paint.net-step-3.png)

+++

@title[Actual paint.net website]

<!-- .slide: data-transition="none" -->
![Build Step](assets/images/install-paint.net-step-4.png)

+++

@title[paint.net download]

<!-- .slide: data-transition="none" -->
![Build Step](assets/images/install-paint.net-step-5.png)

+++

@title[Mirror website]

<!-- .slide: data-transition="none" -->
![Build Step](assets/images/install-paint.net-step-6.png)

+++

@title[Actual paint.net download]

<!-- .slide: data-transition="none" -->
![Build Step](assets/images/install-paint.net-step-7.png)

+++

@title[Unblock zip file]

<!-- .slide: data-transition="none" -->
![Build Step](assets/images/install-paint.net-step-8.png)

+++

@title[Extract zip file]

<!-- .slide: data-transition="none" -->
![Build Step](assets/images/install-paint.net-step-9.png)

+++

@title[Install paint.net]

<!-- .slide: data-transition="none" -->
![Build Step](assets/images/install-paint.net-step-10.png)

+++

@title[paint.net dependencies]

<!-- .slide: data-transition="none" -->
![Build Step](assets/images/install-paint.net-step-11.png)

---

@title[There has to be a better way!]

## "There has to be a better way!"

+++

@title[Chocolatey]

![Chocolatey](assets/images/icon.png)

---

@title[Installing is easy...]

### Installing is easy...

![Build Step](assets/images/install-paint.net-step-12.png)
---

@title[Sane Software Management]

### Chocolatey - Sane Software Management

- Easily manage the software lifecycle
- Native installers, zips and binaries
- PowerShell Module simplifies work
- Packages are independent building blocks
- Integrates with Configuration Management
- Business Friendly Features

---

@title[The Approach]

### Chocolatey - The Approach

- Single, unifying interface - control the chaos
- Decentralized - mulitple places to get packages, including internal
- PowerShell
- Flexible
- Secure
- Reliable

---

@title[Community Package Repository]

### Community Package Repository

- [https://chocolatey.org/packages](https://chocolatey.org/packages)
- Community Feed / Community Maintained
- Moderated as of October 2014
- Everything goes through VirusTotal
- Organisations should NOT depend on this due to trust and control concerns

+++

@title[Community Repository Stats]

![Community Repository](assets/images/community_repo.png)

+++

@title[That is just the beginning...]

### That is just the beginning...

![iceberg](assets/images/Iceberg.jpg)

---

@title[Hosting your own package server]

### Hosting your own package server

- [https://chocolatey.org/docs/how-to-host-feed](https://chocolatey.org/docs/how-to-host-feed)
- Non-Windows Hosting
  - Artifactory
  - Sonatype Nexus
- NuGet Gallery
- ProGet / MyGet
- NuGet.Server / Chocolatey.Server

---

@title[Chocolatey Packages]

### Chocolatey Packages

- Zip files + Versioning, Dependencies & PowerShell
- Metadata Software Information / Package Information
- PowerShell
  - 30+ Built-in functions - turn hard tasks into one-liners
  - Handle additional missing installer logic (like add to PATH)
  - Add options missing from installer arguments
- Files - drop in binaries / native installers

---

@title[Slides/Demos]

## Slides/Demos

### https://gep13.me/ChocolateyDemos

---

@title[Demos]

## Demos

Note:
Mention laptop setup:

---

@title[Only getting started...]

## Only getting started...

- choco upgrade all
- Package Downloader / Internalizer
- Sync with Programs and Features
- Self Service Installer
- Central Management UI / choco deploy
- Package Audit
- Package Reducer
- Install Directory Override
- Download CDN Cache
- Runtime Malware/Virus Protection

---

@title[Questions]

## Questions

Feel free to get in touch

Email: gep13@gep13.co.uk

Twitter: @gep13

Web: https://www.gep13.co.uk

---

@title[Resources]

## Resources

- Chocolatey Documentation - [https://chocolatey.org/docs](https://chocolatey.org/docs)
- Source Code - [https://github.com/chocolatey/choco](https://github.com/chocolatey/choco)
- Learning Resources - [https://chocolatey.org/docs/resources](https://chocolatey.org/docs/resources)
