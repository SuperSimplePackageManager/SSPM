# SSPM
## How simple is SSPM? 
SSPM is arguably too simple, and that's the point.
It's more esoteric than functional, as the goal
is not to make a package manager but rather to make
a super simple package manager.

## Why no options?
Options add clutter. All you do is add what packages
you want to install, and they can be installed.

Installing a package: `sudo sspm install <package>`
Removing a package: `sudo sspm remove <package>`

## Why does SSPM just auto install the package?
Because it adds an extra step, which isn't super
simple.

## Why no dependency checking?
Actually, this one is a personal pet peeve. WHO THE
HELL DECIDED THAT DEPENDENCIES ARE COMPILED **SEPERATELY**
FROM THE PROGRAM!? If your program needs C libraries,
well then tough shit. Should have your make file deal
with it, or make a makefile that uses SSPM to download
dependencies. I am not cluttering my package manager
with a billion libraries. 

## Why no md5 checking?
Who needs checksums? Everything is super reliable!
(That was sarcasm, truth is I didn't feel like it).

## Is this really the most simple?
Probably, idk