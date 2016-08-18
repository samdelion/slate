# > Script

## Script.spawn_prefab

```lua
camera = Script.spawn_prefab("player", Vector3(0, 0, 0));
```

`Entity Script.spawn_prefab(string prefabPath, Vector3 position)`

| Parameter | Type | Description |
|---|---|---|
| prefabPath | string | Path to prefab file to spawn in, excluding .prefab suffix. |
| position | Vector3 | Position to spawn prefab at. |

Create an entity from the given prefab at the given position.

## Script.is\_next_message()

```lua
if (Script.is_next_message()) then
  local msg = Script.next_message()
end
```

`bool Script.is_next_message()`

Returns true if a new message is available for the Lua script and false otherwise.

## Script.next_message()

```lua
if (Script.is_next_message()) then
  local msg = Script.next_message()
end
```

`table Script.next_message()`

Returns a table with the message contents.

## Script.get\_world_transform(Entity entity)

`Matrix4 Script.get_world_transform(Entity entity)`

```lua
local myEntity = Script.spawn_prefab("x", Vector3(0, 0, 0));
local worldTransform = Script.get_world_transform(myEntity);
```

| Parameter | Type | Description |
|---|---|---|
| entity | Entity | Entity to get world transform of. |

Get the world transform of a given entity.

## Script.get\_local_transform(Entity entity)

`Matrix4 Script.get_local_transform(Entity entity)`

```lua
local myEntity = Script.spawn_prefab("x", Vector3(0, 0, 0));
local localTransform = Script.get_local_transform(myEntity);
```

| Parameter | Type | Description |
|---|---|---|
| entity | Entity | Entity to get local transform of. |

Get the local transform (transform relative to parent) of a given entity.

## Script.set\_entity\_animation_index(Entity entity, number animationIndex)

`Script.set_entity_animation_index(Entity entity, number animationIndex)`

```lua
Script.set_entity_animation_index(myEntity, 3);
```

| Parameter | Type | Description |
|---|---|---|
| entity | Entity | Entity to set animation index of. |
| animationIndex | number | Index of animation to play. |

Set the animation that is currently playing for a given entity.

## Script.set\_skybox_material(string skyboxMaterialPath)

`Script.set_skybox_material(string skyboxMaterialPath)`
```lua
Script.set_skybox_material("skyDome01.material");
```

| Parameter | Type | Description |
|---|---|---|
| skyboxMaterialPath | string | Path to material to render skybox with. |

Set the material the skybox is currently being rendered with. 

## Script.create\_gui_panel(number startX, number startY, number endX, number endY, string materialPath)

`Entity Script.create_gui_panel(number startX, number startY, number endX, number endY, string materialPath)`

```lua
guiStartTitlePanel = Script.create_gui_panel(-0.8, 0.9, 0.8, 0.3, "menuTitlePanel.material");
```

| Parameter | Type | Description |
|---|---|---|
| startX | number | Start x-coordinate of the panel. |
| startY | number | Start y-coordinate of the panel. |
| endX | number | End x-coordinate of the panel. |
| endY | number | End y-coordinate of the panel. |
| materialPath | string | Path to material to render panel with. |

Creates a panel (just a non-interactive, 2D UI element).

## Script.create\_gui_button(number startX, number startY, number endX, number endY, string defaultMaterialPath, string pressedMaterialPath, string hoverMaterialPath)

`Entity Script.create_gui_button(number startX, number startY, number endX, number endY, string defaultMaterialPath, string pressedMaterialPath, string hoverMaterialPath)`

```lua
guiToggleHardModeButton = Script.create_gui_button(-0.10, -0.20, 0.10, -0.40,  "s_difficulty_default.material", "s_difficulty_pressed.material", "s_difficulty_hover.material");
```

| Parameter | Type | Description |
|---|---|---|
| startX | number | Start x-coordinate of the panel. |
| startY | number | Start y-coordinate of the panel. |
| endX | number | End x-coordinate of the panel. |
| endY | number | End y-coordinate of the panel. |
| defaultMaterialPath | string | Material to render with if button isn't pressed or hovered over. |
| pressedMaterialPath | string | Material to render with if button is pressed. |
| hoverMaterialPath | string | Material to render with if button is hovered over. |

Creates a gui button that sends button press events.

## Script.get\_local_translation(Entity entity)

`Vector3 Script.get_local_translation(Entity entity)`

```lua
local chaserTranslate = Script.get_local_translation(chaser);
```

| Parameter | Type | Description |
|---|---|---|
| entity | Entity | Entity to set the local translation of. |

Get the local translation (translation relative to parent) of the given entity.

## Script.get\_world_translation(Entity entity)

`Vector3 Script.get_world_translation(Entity entity)`

```lua
local chaserWTranslate = Script.get_world_translation(chaser);
```

| Parameter | Type | Description |
|---|---|---|
| entity | Entity | Entity to set the world translation of. |

Get the world translation (translation relative to world coordinate system) of the given entity.

## Script.get\_local_scale(Entity entity)

`Vector3 Script.get_local_scale(Entity entity)`

```lua
local chaserScale = Script.get_local_scale(chaser);
```

| Parameter | Type | Description |
|---|---|---|
| entity | Entity | Entity to set the local scale of. |

Get the local scale of the given entity.

## Script.get\_world_scale(Entity entity)

`Vector3 Script.get_world_scale(Entity entity)`

```lua
local chaserWScale = Script.get_world_scale(chaser);
```

| Parameter | Type | Description |
|---|---|---|
| entity | Entity | Entity to get the world scale of. |

Get the world scale of the given entity.

## Script.set\_local_scale(Entity entity, Vector3 scale)

`Vector3 Script.set_local_scale(Entity entity, Vector3 scale)`

```lua
Script.set_local_scale(trigger_area, Vector3(5.0, 5.0, 5.0));
```

| Parameter | Type | Description |
|---|---|---|
| entity | Entity | Entity to set the local scale of. |
| scale | Vector3 | New scale to set. |

Set the local scale of the given entity.

## Script.get\_local_orientation(Entity entity)

`Quaternion Script.get_local_orientation(Entity entity)`

```lua
localOrientation = Script.get_local_orientation(player);
```

| Parameter | Type | Description |
|---|---|---|
| entity | Entity | Entity to set the local orientation of. |

Get the local orientation of the given entity.

## Script.get\_world_orientation(Entity entity)

`Quaternion Script.get_world_orientation(Entity entity)`

```lua
worldOrientation = Script.get_world_orientation(player);
```

| Parameter | Type | Description |
|---|---|---|
| entity | Entity | Entity to get the world orientation of. |

Get the world orientation of the given entity.

## Script.set\_local_orientation(Entity entity, Quaternion orientation)

`Quaternion Script.set_local_orientation(Entity entity, Quaternion orientation)`

```lua
Script.set_local_translation(ent, myRot);
```

| Parameter | Type | Description |
|---|---|---|
| entity | Entity | Entity to set the local orientation of. |
| orientation | Quaternion | New orientation to set. |

Set the local orientation of the given entity.

## Script.destroy_entity(Entity entity)

`Script.destroy_entity(Entity entity)`

```lua
Script.destroy_entity(guiStartPlayButton)
```

| Parameter | Type | Description |
|---|---|---|
| entity | Entity | Entity to destroy. |

Send a message to all systems, telling them to destroy the given entity.

## Script.set\_material_parameter(string materialResourceFilePath, string parameterName, string parameterType, any data)

`Script.set_material_parameter(string materialResourceFilePath, string parameterName, string parameterType, any data)`

```lua
Script.set_material_parameter("colour.material", "u_colour", "vec4", Vector4(0.8, 0.8, 0.8, 1.0))
```

| Parameter | Type | Description |
|---|---|---|
| materialResourceFilePath | string | Material to set parameter of. |
| parameterName | string | Parameter in material to manipulate. |
| parameterType | string | Type of parameter (vec4, int, mat4, float). |
| data | any | New data to give to parameter. |

Set the value of a parameter in a given material.

## Script.quit()

`Script.quit()`

```lua
Script.quit() -- Shutdown everything 
```

Sends a quit message to all systems, telling them to shutdown. Shuts down the engine.

## Script.set_pause(bool shouldPause)

```lua
Script.set_pause(true); -- Pause game
Script.set_pause(false); -- Unpause game
```

`Script.set_pause(bool shouldPause)`

| Parameter | Type | Description |
|---|---|---|
| shouldPause | bool | true to pause, false to unpause. |

Systems will receive pause message, up to them whether they should pause or not.
