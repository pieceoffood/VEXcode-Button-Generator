# VEXcode Button Generator + template for the VEX V5 brain

### This is a WORK IN PROGRESS, expect the unexpected

The VEXcode Button Generator consists of a class designed to automate the process of adding a button to the V5 Brain screen in VEXcode.  It is meant to help new users get started with the V5 system, not as a tool for advanced porgrammers.  It can, however, be a handy tool for quickly making autonomous selectors or control the robot from the brain itself.
With it you can create a button with automatically centered text and press detection in one line and change button attributes on the fly.

___

**To add to currently existing project:** download the ButtonClass.h file itself and add ```#include "ButtonClass.h"``` to files that it will be used in.

**To download the template:** download the ButtonMakerTemplate folder and open the contained .v5code file

___


### Button attributes:
 - centered position in coordinate plane
 - button color
 - button dimensions
 - button color in hue (int), hex (string, ie "#FFFFFF"), or a preset color (string, ie "white")
 - outline color in hue (int), hex (string, ie "#FFFFFF"), or a preset color (string, ie "white")
 - outline thickness
 - text inside button


WIP:
 - use custom images from SD card
 - text font
 - text size

### Limitations:
Press detection is limited to rectangular shapes, it cannot accurately detect presses for other shapes.

Cannot delete previously drawn buttons or automatically redraw a button - to display changes in a button the screen must be cleared and then be redrawn with button.draw(); while the press detection changes immediately after being updated.  This is due to the screen's inability to identify objects.  Any deletion of objects would hae to clear the entire screen.
