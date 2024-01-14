---
layout: single
title:  "Customizing Shortcuts in Blueprints"
category: Editor tips
tags:
    - Editor
    - Programming
    - UE5
---

When working with blueprints, you've likely encountered handy shortcuts like `B + LMB` (place branch node) or `S + LMB` (sequence node). What you might not be aware of is the ability to customize your own shortcuts for both the blueprint graph and the material graph.

Let's take the example of setting a shortcut for the `Print String` node to `R + LMB`. To implement a shortcut, locate the file ```[your engine installation dir]\Engine\Config\BaseEditorPerProjectUserSettings.ini```, and navigate to the `[BlueprintSpawnNodes]` section for the blueprint graph or `[MaterialEditorSpawnNodes]` for the material graph.

For the Print String node, the syntax is as follows: ```+Node=(Class=KismetSystemLibrary:PrintString Key=R Shift=false Ctrl=false Alt=false)```.

By following this approach, you can assign keyboard shortcuts to various *engine* functions and events.