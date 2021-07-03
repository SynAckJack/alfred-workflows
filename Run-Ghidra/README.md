# Run-Ghidra

## Overview

Just a little script to run Ghidra from Alfred.

Uses the `ghidra` keyword and accepts a variable for the path to a project file, if required:

`gihdra <PATH>`

Although, it is optional and it can simply be run as: 

`ghidra`

## Requirements

So this of course requires Ghidra to be installed. This has only been tested with Ghidra installed through brew:

`$ brew install --cask ghidra`

which creates the symlink:

`/usr/local/bin/ghidraRun -> Install Location`

This script relies on that symlink due to the limitations of accessing the `$PATH` from an Alfred script (although any feedback on that would be great).
