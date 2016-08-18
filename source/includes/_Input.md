# > Input 

## Input.is\_key_pressed(string keyName)

```lua
if (Input.is_key_pressed("w")) then
  print("W pressed")
end
```

`bool Input.is_key_pressed(string keyName)`

| Parameter | Type | Description |
|---|---|---|
| keyName | string | Name of key to check if pressed. |

Returns true if the given key is pressed and false otherwise.

## Input.get\_mouse\_delta_xy()

```lua
dX, dY = Input.get_mouse_delta_xy()
```

`deltaX, deltaY Input.get_mouse_delta_xy()`

Returns the amount (in pixels) the mouse has moved since the last frame.
