---
uid: "contribution/vl.elementa"
uid-meta: "contribution/vl.elementa-meta"
comments: 
 items: 
  - uid: "275466"
  - uid: "275467"
  - uid: "275484"
  - uid: "275485"
  - uid: "276551"
title: "VL.Elementa"
image: "ElementaThumb.png"
contribution: "true"
---

A node based UI widgets library made in VL for Skia rendering.

The library includes:
- a collection of ready to use widgets to handle the most common value types in vvvv Gamma
- a set of Layout nodes to easily arrange your widgets and create responsive UIs
- a bunch of utilities and help patches


1.  Installing
To use the latest stable version: 
1. go to Gamma's Quad menu > Manage Nugets > Commandline
2. type this:
 ``` 
nuget install vl.elementa 
```
3. press Enter and wait the ending of the installation process


1.  Contributing to the development
1. Clone the repository <https://github.com/vvvv-dottore/VL.Elementa>
1. build the solution located in the `src` folder in `Release` mode. 
1. You can then start contributing to the lib.

1.  Resources
Repository <https://github.com/vvvv-dottore/VL.Elementa>
Chat Room <https://riot.im/app/#/room/#VL.Elementa:matrix.org>

1.  Licencing
MIT License - You're free to use VL.Elementa in your creative & commercial projects.

[Natan Sinigaglia](http://natansinigaglia.com/)


1.  Changelog
###  2.2.2
- Panel fix

###  2.2.1
- Cleanup in the node browser
- some fixes

###  2.2.0
- New LayerElementum widget
- New Drawable component
- Drawing performance improved
###  2.1.1
- New Image node
- Fixes in help patches

###  2.1.0
- New Panel node
- New Folder node
- New Style utility nodes
- New Tooltip component
- Added GetStyleSheet operation in IElementum
- Added GetComponentsVersion in IElementum
- Changed GetDirtyLayout and GetDirtyGraph operations in IElementum to GetLayoutVersion and GetGraphVersion
- Introduced ElementaContext class: every widget have access to the graph resources
- Added SetElementaContext and SetMe operations in IElementum
- Introduced SetElementaContext and SetParent operations in IComponent: each component has now access to any resource of the graph and can easily edit its own parent widget
- Different Layout/Graph/Components changes check system
- Help patches now referencing the nuget instead of the vl file (SavingAs the patches doesn't break the reference)
- Cleaned Root node architecture
- fixed Moveable and Resizeable components behaviour in multi selection scenarios
- New componentProcessors management
- Individual help patches available for all widgets
- Added node and pin descriptions on all widgets
- Reorganized help patches
- Deleted TextFieldMultiline, which is now TextField
- Some minor fixes

###  2.0.0
- New nodes to push widgets to Overlay
- Renamed the library to VL.Elementa
- New widget architecture : value properties and widget manager are now generic
- completely reworked StyleSheet management
- Style can be provided to a widget with the new Styleable component
- Orientation, multi-components widgets and specific attributes are now handled by components (was in widget managers before)
- Widgets can now have custom drawers
- Layout nodes (stack, columns, etc) now provide more options to play with, allowing more precise layout
- Added Padding to layout nodes
- A widget's ValueProperty can be provided from outside, allowing several widgets to share the same ValueProperty
- mapping between external ValueProperties of different types
- New help patches explaining custom drawers, shared value properties and Moveable/Resizeable components

###  1.0.0
- First version of the architecture