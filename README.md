# MINGW-packages
[![Discord](https://img.shields.io/discord/937821572285206659?style=flat-square&label=Discord&logo=discord&logoColor=white&color=7289DA)](https://discord.gg/JBUgcwvpfc)

This repository contains package scripts to build under MSYS2 [TEK environment](https://github.com/teknology-hub/MinGW-env).

It's forked from [MSYS2's repository](https://github.com/msys2/MINGW-packages) with the following changes:
- Only packages required for building TEK software are included
- All PKGBUILDs are brought to the same style
- Build options for most packages are tweaked to disable unnecessary dependencies (or enable ones needed for TEK software), enable static library building where it wasn't properly enabled upstream, and fix build issues
- Some packages got extra patches to accomodate the above changes
- All packages are stripped of files not involved in building (docs, manpages, etc). The idea is having a minmalistic build environment rather than a full-fledged delelopment one

There is no intention to keep this repository in sync with upstream, it will be updated once in a while

The repository hosting binary packages is available at https://teknology-hub.com/software/mingw/tek-x86_64/. It's signed by Nuclearist's [GPG key](https://teknology-hub.com/public-keys/gpg/nuclearist.asc)
