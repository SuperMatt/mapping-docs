---
title: "func_detail"
date: 2024-08-15T13:44:21+01:00
draft: false
---

In order to speed up rendering, Quake engine games use an entity type called `func_detail`. This entity type is used to mark brushes that are not part of the world geometry, but are still visible to the player. Think of world geometry as the walls, floors, and ceilings that make up the level, and `func_detail` as the props , decorations and stairs that are placed on top of the [World Geometry]({{< ref "world_geometry" >}})

When the engine renders a level, it first processes the world geometry, and then it processes the `func_detail` entities. This allows the engine to render the level more quickly, because it doesn't have to render the `func_detail` entities until after the world geometry is done.
