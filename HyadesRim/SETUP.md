# BattleTech Mod Installation Guide

## Table of Contents

- [ModTek Download](#modtek-download)
- [Hyades Rim Download](#hyades-rim-download)
- [CAB-3025 Download](#cab-3025-download)
- [File Changes](#file-changes)
    - [Dependency Resolution](#dependency-resolution)
- [CleverGirl Download](#clevergirl-download)
    - [Dependency: IRBTModUtils Download](#dependency-irbtmodutils-download)
    - [Dependency: Custom Ammo Categories Download](#dependency-custom-ammo-categories-download)
- [CustomUnits Dependency Conflict Resolution](#customunits-dependency-conflict-resolution)
- [IRTweaks Download](#irtweaks-download)

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

## CleverGirl Download

1. Go to [CleverGirl Releases](https://github.com/BattletechModders/CleverGirl/releases)
2. Download the latest release
3. Extract the downloaded archive to your BattleTech game mods folder

### Dependency: IRBTModUtils Download

1. Go to [IRBTModUtils Releases](https://github.com/BattletechModders/IRBTModUtils/releases)
2. Download the latest release
3. Extract the downloaded archive to your BattleTech game mods folder
4. Modify hidden property to be false in the mod.json file

### Dependency: Custom Ammo Categories Download

1. The repo releases section is very out of date [Custom Ammo Categories Releases](https://github.com/BattletechModders/CustomAmmoCategories/releases)
   1. Latest release is 0.1.49 from 20190520, but BTA3062-light uses 0.0.1.205 from 20191001. 
2. For now, going to use BTA3062-light from 20191001.
3. Download the latest release from [BTA3062-light downloader](https://www.bta3062.com/files/BTAdvancedLauncher.php)
   1. I'll figure out where the launcher is getting the mod from later (if this works)
4. Grab the Mods folder and store it in a backup file.
5. Modify hidden property to be false in the mod.json file
6. Repeat steps 1-5 for the other mod dependencies:
   1. CustomLocalization,
      CustomLocalSettings,
      CustomPrewarm,
      CustomComponents,
      CustomAmmoCategories,
      CustomUnits,
      CBTBehaviorsEnhanced,
      CustomVoices

### CustomUnits Dependency Conflict Resolution

To resolve the conflict between CustomUnits and MechResizer:

1. Locate the MechResizer mod in your BattleTech game mods folder
2. Delete the MechResizer mod folder completely
3. Does it work? Will update this section if it does not

## IRTweaks Download

1. Go to [IRTweaks Releases](https://github.com/BattletechModders/IRTweaks/releases)
2. Download the latest release
3. Extract the downloaded archive to your BattleTech game mods folder
4. In mod.json, modify "DisableCampaign" to be false




