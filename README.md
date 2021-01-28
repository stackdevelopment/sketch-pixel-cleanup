# Pixel Cleanup For Sketch

- This repository is no longer supported! Please feel free to fork and update if it isn't working with your version of Sketch.

One of the best things about Sketch is having your designs be pixel perfect. However, there are a variety of things that can end up with pesky portion-of-a-pixel positioning.

This beta plugin will round all of your pixels to whole pixels.

It works well for the following:

1. Lines
1. Rectangles
1. Circles
1. Groups
1. Nested groups

Working but not extensively tested:

2. Symbols
2. Complex paths

Untested:

3. Images
3. Extensive edge cases such as scaling + rotation. 
3. Compound shapes
3. Masks
3. Anything not listed above


It may work with others, but I haven't tested it fully.

### Instructions

1. Select 1 or more layers or groups
2. Press the keyboard shortcut`option-command-p`
3. Bask in the whole pixel glory. 

### Things To Know
• If a shape is in a group, it is possible that `both the shape, and the group itself may have been positioned\shaped at partial pixels`. 

If you do select a shape in a group and run the command, it will adjust all parent groups and the shape, but it will not not automatically adjust the other sibling shapes. It's easy enough to add that as a feature, but I wanted to avoid unintended consequences. Sometimes you really do mean to have partial pixel placement.

• If you select a group and run the command this will clean up `the group AND all of its children, and all sub groups, and all of THEIR children`

Note: In Sketch, the inspector doesn't instantly update refresh when these properties are changed, so though things will move correctly, you have to deselect/reselect to see the change in the inspector. I didn't auto-deselect so you wouldn't loose your initial selection. 

All feedback and issues are welcome!
Happy pixel hunting!
#### Obligitory Warning
This is a beta. Use at your own risk.
It's generally good practice anyway but use version control before trying this out on an important document


