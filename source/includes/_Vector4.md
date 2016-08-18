# > Vector4

## Vector4

```lua
local vec = Vector4(4, 0.1, 3.0, 1.0);
```

`Vector4 Vector4(number x, number y, number z, number w)`

| Parameter | Type | Description |
|---|---|---|
| x | number | x component of Vector4. |
| y | number | y component of Vector4. |
| z | number | z component of Vector4. |
| w | number | w component of Vector4. |

Construct a Vector4 from the given components.

## Vector4.new(number x, number y, number z, number w)

```lua
local vec = Vector4.new(4, 0.1, 3.0, 1.0);
```

`Vector4 Vector4.new(number x, number y, number z, number w)`

| Parameter | Type | Description |
|---|---|---|
| x | number | x component of Vector4. |
| y | number | y component of Vector4. |
| z | number | z component of Vector4. |
| w | number | w component of Vector4. |

Construct a Vector4 from the given components.

## Vector4.magnitude(Vector4 v)

```lua
local wishDir = Vector4(0, 0.1, 0, 1.0);
if (Vector4.magnitude(wishDir) > 0) then
   print("Do stuff")
end
```

`number Vector4.magnitude(Vector4 v)`

| Parameter | Type | Description |
|---|---|---|
| v | Vector4 | Vector4 to find magnitude of. |

Return the magnitude of the given Vector4.

## Vector4.normalize(Vector4 v)

```lua
local wishDir = Vector4(0, 0.1, 0, 1.0);
wishDir = Vector4.normalize(wishDir);
```

`Vector4 Vector4.normalize(Vector4 v)`

| Parameter | Type | Description |
|---|---|---|
| v | Vector4 | Vector4 to normalize. |

Return a normalized version of the given Vector4.

## Vector4.invert(Vector4 v)

```lua
local vec = Vector4(1, 0, 1, 1);
print(vec); -- {1, 0, 1, 1}
local vec = Vector4.invert(vec);
print(vec); -- {-1, 0, -1, -1}
```

`Vector4 Vector4.invert(Vector4 v)`

| Parameter | Type | Description |
|---|---|---|
| v | Vector4 | Vector4 to invert. |

Return an inverted version of the given Vector4.

## Vector4.dot(Vector4 v1, Vector4 v2)

```lua
local v1 = Vector4(0, 1, 0, 1);
local v2 = Vector4(0, 1, 0, 1);
local dot = Vector4.dot(v1, v2); -- 2 
```

`number Vector4.dot(Vector4 v1, Vector4 v2)`

| Parameter | Type | Description |
|---|---|---|
| v1 | Vector4 | Vector4 to dot product. |
| v2 | Vector4 | Vector4 to dot product. |

Return the dot product of the two given vectors.

## Vector4.transform(Vector4 v, Matrix4 m)

```lua
local vecTransformed = Vector4.transform(myVec, myMatrix);
```

| Parameter | Type | Description |
|---|---|---|
| v | Vector4 | Vector4 to transform. |
| m | Matrix4 | Matrix4 to transform Vector4 by. |

Return a Vector4 equal to the given Vector4 transformed by the given Matrix4.

## Vector4.unit_x()

```lua
local unitX = Vector4.unit_x() -- {1, 0, 0, 0}
```

`Vector4 Vector4.unit_x()`

Return a Vector4 of magnitude 1 in the x-direction.

## Vector4.unit_y()

```lua
local unitY = Vector4.unit_y() -- {0, 1, 0, 0}
```

`Vector4 Vector4.unit_y()`

Return a Vector4 of magnitude 1 in the y-direction.

## Vector4.unit_z()

```lua
local unitZ = Vector4.unit_z() -- {0, 0, 1, 0}
```

`Vector4 Vector4.unit_z()`

Return a Vector4 of magnitude 1 in the z-direction.

## Vector4.unit_w()

```lua
local unitW = Vector4.unit_w() -- {0, 0, 1, 0}
```

`Vector4 Vector4.unit_w()`

Return a Vector4 of magnitude 1 in the w-direction.

## Vector4:get_x()

```lua
local vec = Vector4(3.14159, 0, 0, 1);
local x = vec:get_x(); -- 3.14159
```

`number Vector4:get_x()`

Return the x component of the given Vector4.

## Vector4:get_y()

```lua
local vec = Vector4(0, 3.14159, 0, 1);
local y = vec:get_y(); -- 3.14159
```

`number Vector4:get_y()`

Return the y component of the given Vector4.

## Vector4:get_z()

```lua
local vec = Vector4(0, 0, 3.14159, 1);
local z = vec:get_z(); -- 3.14159
```

`number Vector4:get_z()`

Return the z component of the given Vector4.

## Vector4:get_w()

```lua
local vec = Vector4(0, 0, 3.14159, 1);
local w = vec:get_w(); -- 1 
```

`number Vector4:get_w()`

Return the w component of the given Vector4.

## Vector4:set_x()

```lua
local vec = Vector4(0, 0, 0, 1); -- {0, 0, 0, 1}
vec:set_x(3.14159); -- {3.14159, 0, 0, 1}
```

`Vector4:set_x(number x)`

| Parameter | Type | Description |
|---|---|---|
| x | number | Value to given to x component of given Vector4. |

Set the x component of the given Vector4 to the given value.

## Vector4:set_y()

```lua
local vec = Vector4(0, 0, 0, 1); -- {0, 0, 0, 1}
vec:set_y(3.14159); -- {0, 3.14159, 0, 1}
```

`Vector4:set_y(number y)`

| Parameter | Type | Description |
|---|---|---|
| y | number | Value to given to y component of given Vector4. |

Set the y component of the given Vector4 to the given value.

## Vector4:set_z()

```lua
local vec = Vector4(0, 0, 0); -- {0, 0, 0, 1}
vec:set_z(3.14159); -- {0, 0, 3.14159, 1}
```

`Vector4:set_z(number z)`

| Parameter | Tzpe | Description |
|---|---|---|
| z | number | Value to given to z component of given Vector4. |

Set the z component of the given Vector4 to the given value.

## Vector4:set_w()

```lua
local vec = Vector4(0, 0, 0); -- {0, 0, 0, 1}
vec:set_w(3.14159); -- {0, 0, 0, 3.14159}
```

`Vector4:set_w(number w)`

| Parameter | Twpe | Description |
|---|---|---|
| w | number | Value to given to w component of given Vector4. |

Set the w component of the given Vector4 to the given value.
