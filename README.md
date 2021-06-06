# GN Simple Build Example

## Warning

This copy works fine on mid 2021, things gona be changed after

## prepare

+ have [depot_tools](https://www.chromium.org/developers/how-tos/get-the-code) installed
+ If Windows download [Cygwin](http://cygwin.com/install.html) to let gcc/g++/rm been installed

## Description
This is an example directory structure that compiles some simple targets using
gcc. It is intended to show how to set up a simple GN build. It is deliberately
simplistic so the structure is more clear, and doesn't support everything on
every platform.

It is recommended that you take this and add on as your requirements indicate.
You may also want to see the Chromium and Fuchsia build configurations for the
maximal functionality (the [root README](../../README.md) has links to these).

Don't miss the ".gn" file in this directory which may be hidden on your system!

## Usage

```bash
gclient config --unmanaged https://github.com/browser-dev/gn-simple-build.git --name=src
```
```bash
gclient sync
```
```bash
gn gen out
```
```bash
ninja -C out
```
