---
layout: post
title:  "How to create shortcuts to place nodes"
category: Editor tips
tags:
    - Editor
    - Programming
    - UE5
---

When using blueprints, you have probably come across shortcuts such as `B + LMB` (place branch node) or `S + LMB` (squence node). What you might not know is that you can create such shortcuts yourself - for both the blueprint graph and the material graph.

As an example, we will use `Print String` with a shortcut of `R + LMB`. To add a shortcut, find the file [your engine installation dir]\Engine\Config\BaseEditorPerProjectUserSettings.ini and find the section [BlueprintSpawnNodes] for blueprint graph and [MaterialEditorSpawnNodes] for material graph. 

Syntax for the `Print String` node: `+Node=(Class=KismetSystemLibrary:PrintString Key=R Shift=false Ctrl=false Alt=false)`. 

This way you can use a keyboard shortcut for any engine function/event.