# spm
### Simple Package Manager

---

To allow software to be gracefully added and removed, spm exists.
- We may intend to use spm for update functionality, but that has to be implemented yet.

#### The default repo for OS/1337 is:
https://github.com/OS-1337/pkgs

---
##  FAQ

### Why spm?
####  Because all package managers suck!
Okay, that's sarcasm and yum as well as apt are great, but they are way too *THICC* for [OS/1337](https://os1337.com) and thus a sleeker alternative is necessary.
- And being able to just *yoink* binaries from the [OS/1337 package repository](https://github.com/OS-1337/pkgs) is what it should do. 
###

### How simple is spm? 
spm is arguably too simple, and that's the point.
- The intended design is to be brutally simple!
###

### Why no options?
#### Options add clutter!
All you do is add what packages  you want to install, and they can be installed.
- Installing a package: `sudo spm install <package>`
- Removing a package: `sudo spm remove <package>`
###

### Why does spm just auto install the package?
Because it adds an extra step, which isn't super simple.
###

### Why no dependency checking?
Actually, this one is a personal pet peeve of the [SSPM project's maintainer](https://github.com/SuperSimplePackageManager/SSPM):
#### "WHO THE HELL DECIDED THAT DEPENDENCIES ARE COMPILED ***SEPERATELY*** FROM THE PROGRAM!?"
If your program needs C libraries, well then that's your problem! 
- Should have your make - file deal with it, or make a makefile that uses spm to download dependencies.
  - We won't clutter the package manager with a billion libraries!

Also as Linus Torvalds said:
#### ["WE DO NOT BREAK USERSPACE!"](https://lkml.org/lkml/2012/12/23/75)
- Which is something Glibc constantly violates and which is why it's absolutely trash for every CCSS!
###

### Why no MD5 / signature checking?
Who needs checksums or signatures? Everything is super reliable!
- That was sarcasm, truth is I didn't feel like adding it in yet.
###

### Is this really the most simple?
Probably not, as [SSPM](https://github.com/SuperSimplePackageManager/SSPM) will likely be simpler, and is the source that has been [forked here](https://github.com/OS-1337/spm).
###