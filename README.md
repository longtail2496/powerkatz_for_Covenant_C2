﻿# PowerKatz DLLs for Covenant C2

## What is this repository for ?
Mimikatz is a built-in task in Covenant C2 that uses SharpSploit project, current version of Mimikatz in the project is very old and and does not work on new OSs. We can update those DLLs manually in Covenant C2.

## Steps:
- Download both DLLs from this repository to local system.
- Copy and paste the files in `Covenant/Covenant/Data/EmbeddedResources/` directory.

> NOTE: I can not gurrantee that these files in this repository were compiled correctly, thus if anyone want to use these files in any real engagements\exams, please compile by following the below steps as I cannot gurrantee the accuracy of any files. I have just kept these files for my personal reference

## How were these DLLs obtained ?
- Microsoft Visual Studio 2019 was installed along with WDK
- Mimikatz repository from https://github.com/gentilkiwi/mimikatz was cloned using git clone command
- The Projcet's solution file (.sln) was opened in Visual Studio
- The solution configurations was used is "Second_Release_PowerShell"
- These DLLs were built for x64 and x86 architectures by selecting solution platforms 'x64' and 'Win32' respectively
- We need to build the project two times for each architecture
- Both 64 bit and 32 bit `powerkatz.dll` were copied in a directory and named accordingly (as can be seen in the repo)

## Instructions
These above mentioned process is from [Pentester Academy's Attacking Active Directory series](https://bootcamps.pentesteracademy.com/certifications) of courses and are documented in lab manual. These repo is maintained to avoid to configure a build environement each time these files are needed.

