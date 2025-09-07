# BattleTech Mod Installation Guide

## Table of Contents

- [ModTek Download](#modtek-download)
- [Hyades Rim Download](#hyades-rim-download)
- [CAB-3025 Download](#cab-3025-download)
- [File Changes](#file-changes)
- [Dependency Resolution](#dependency-resolution)

## ModTek Download

1. Download the latest version of ModTek from [ModTek Releases](https://github.com/BattletechModders/ModTek/releases)
2. Follow the [ModTek Installation Guide](https://github.com/BattletechModders/ModTek/blob/master/INSTALL.md) for
   detailed installation instructions

## Hyades Rim Download

1. Go to [Hyades Rim on Nexus Mods](https://www.nexusmods.com/battletech/mods/473)
2. Download the latest version of the mod by clicking the "Manual Download" button
3. Extract the downloaded archive to your BattleTech game mods folder

<!-- Instructions for downloading Hyades Rim mod will go here -->

## CAB-3025 Download

1. Go to [CAB-3025 Repository](https://github.com/BattletechModders/CAB-3025) on GitHub
2. Download CAB-3025 Repo
3. Extract the downloaded archive
4. Copy the "CAB-3025" directory from the extracted folder to your BattleTech game mods folder

## File Changes

### Dependency Resolution

To resolve the circular dependency issue between CAB-3025-HyadesRim and MechResizer:

1. Locate the mod.json file in your CAB-3025-HyadesRim mod folder
2. Open the file in a text editor
3. Remove the "MechResizer" entry from the "DependsOn" section
4. Save the file

