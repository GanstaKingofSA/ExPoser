# Welcome to ExPoser!

ExPoser is a WIP expression tool based off u/chronoshag's Mood Pose Tool (MPT) that attempts to fix MPT related bugs and provide a easier posing experience for Ren'Py 7 modders whether they are new to modding or not.

## Features
- New Syntaxes for newcomers and advanced users of Ren'Py 7 and/or Mood Pose Tool
- Natural Blinking Expression Integration Support
   > As of today, you have to install NBE's asset files (not the RPY code) onto your mod project and uncomment the `blink` group in each characters' layeredimage file in order for NBE to work.

## What has changed from MPT?
All code in ExPoser is based off MPT and should work the same as intended for all projects except for one condition.

Many users have communicated some issues in regards to how MPT separates a special pose and a base pose. Mood Pose Tool normally defines the special poses fine such as `tap`, `lean`, `cross` for Sayori, Monika and Natsuki, but for base poses, it changes it to be a unusual mix of `turned` for Sayori, Natsuki and Yuri and `forward` for Monika alone. 

ExPoser addresses this by renaming these `turned`/`forward` to `base` which stands for their normal poses (don't confuse this for their outfits). Due to this, if you are transferring from MPT to ExPoser, you will need to change the MPT syntax over to ExPoser's new syntax.

Example:

In Mood Pose Tool you will call a awkward Sayori as such.
```py
show sayori turned casual awkw
```
In ExPoser however, you will call Sayori like this instead
```py
show sayori base casual awkw
```

Additionally there is now new syntaxes available that actually makes posing easier to understand with actual english words to describe the poses themselves over the traditional MPT syntax for newcomers to get into modding.

Example:

In Mood Pose Tool you will call a awkward Sayori as such.
```py
show sayori turned casual awkw
```
In ExPoser however, you will call Sayori like this instead
```py
show sayori base casual awkward
```
You can still use the MPT syntax however. This is just a easier way to call it for newcomers than referring to a long guide list and trying to understand each var for debugging purposes.

There are a lot of new syntax changes to cover so if you are interested in getting started, why not look at the new syntax available in this [PDF](New%20Tool%20Syntax%20Guide.pdf) file and learn how to use ExPoser for your daily needs.

## What do you need to use ExPoser
1. A mod you are working on.
2. MPT 1.1.1 (for the layeredimage images)
   > Due to lack of permissions to distribute MPT assets with ExPoser, you will need MPT to copy the layeredimages folders for each character from within `the MPT ZIP file/game/mod_assets/MPT` over to ExPoser in `your mod folder/game/mod_assets/MPT`.
3. (Optional) Natural Blinking Expressions

## Install Guide
1. Install MPT over your mod.
2. Open ExPoser's ZIP file, and copy all of it's assets over to your mod. Replace any files if requested.
3. (Optional) Copy the characters' folders in `the NBE ZIP folder/game/mod_assets/MPT` over to ExPoser in `your mod folder/game/mod_assets/MPT`.
4. (If you did step 3) Uncommment the `blink` groups in each characters' layered image RPY file.
4. Done!

## Credits
- u/ZachmanAwesomenessII - Fixed Poses for Natsuki's `fta`/`turned_away_face` pose.
- Willinisian - Natural Blinking Expressions Code
- MPT Team - Mood Pose Tool Syntax Code
- u/retroadamshow-1 and Kae (Discord) for testing.

Copyright 2022 GanstaKingofSA. All rights reserved. The ExPoser project is unaffiliated with the Mood Pose Tool team and Team Salvato. 
