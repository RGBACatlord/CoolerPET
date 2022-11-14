# CoolerPET
This is a custom build of the Source Engine particle editor, tailored to creation of Team Fortress 2 unusual effects.
*UPDATE:* Unfortunately, recent updates to tf2 have changed something somewhere which has broken CPET. It was a fun ride gamers.

# New Features
Some of these features are unique to CPET while others are simply ported from new engine branches.
Features are as follows:

* AutoView
  * When enabled, the particle preview window will zoom and position the view based off the particle system's bounding box.
* Lock Preview
  * When on, the particle preview will stay viewing the selected system, so you can work on children and see how it affects the parent.
* Some new general toggles
  * Render Axes (Helpful for workshop images/videos)
  * Render Control Points (Renders axes at all CPs)
  * Render Grid
* Keyboard Shortcuts
  * Definition Browser
    * 1: New System
    * 2: Copy Selected System
  * Particle Preview
    * 1: Toggle Axes
    * 2: Toggle AutoView
    * 3: Toggle Grid
    * 4: Toggle CP Axes
    * 5: Restart the preview
  * These can be disabled by tool window or globally with
```cpet_disable_keybinds_(all/modelpreview/systembrowser/particlepreview)```
* Console
  * Adds a better console page to the mini viewport
* Particle Definition Browser
  * Added Copy and Replace
    * Will duplicate selected systems and replace every occurence of a word with another
    * Child Highlighting: Children of the selected definition will be highlighted
* Properties
  * Booleans show as true or false now (Disable with cpet_properties_bool_as_text 0), and takes 'true' and 'false' as valid values.
  * Custom properties window colors can be set through the CoolerPET menu button
  * Added Keybinds
    * 1: Add new function
    * A: Move selected function up
    * D: Move selected function down
* Model Preview
  * Adds an entirely new tool window to PET: see how the effect looks on a player in-editor
  * Includes a slider for effect Z offset
  * ```cpet_mdl_test_offset_(x/y/z)``` int (default 0): Particle system offset
  * ```cpet_mdl_realign_on_change``` 0/1 (default 1): Reset camera on class/anim change

# Installation

Drag the "Team Fortress 2" folder into your steamapps/common and replace all.
CoolerPET will now appear in your tools list, along with the vanilla particle editor.

Your particle editor's layout might be slightly screwed on first launch - fix it with View->Default Layout

# FAQ

**Will this trigger VAC?**

*It's very unlikely as it uses the source tool framework as intended,
but I'd still recommend you run it insecure just to be super safe.
At the end of the day, you run this at your own risk!*

**Can you add X feature / fix X bug?**

*Probably. Go ahead and start an issue and I'll take a look.*

**Is Valve ok with this?**

*I asked Valve directly and I'm still waiting for a reply, so I can only assume they don't care!*
