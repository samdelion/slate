# > Vector3

## Vector3

```lua
local wishDir = Vector3(0, 0.1, 0);
```

`Vector3 Vector3(number x, number y, number z)`

| Parameter | Type | Description |
|---|---|---|
| x | number | x-component of Vector3. |
| y | number | y-component of Vector3. |
| z | number | z-component of Vector3. |

Construct a Vector3 from the given components.

## Vector3.new(number x, number y, number z)

```lua
local wishDir = Vector3.new(0, 0.1, 0);
```

`Vector3 Vector3.new(number x, number y, number z)`

| Parameter | Type | Description |
|---|---|---|
| x | number | x-component of Vector3. |
| y | number | y-component of Vector3. |
| z | number | z-component of Vector3. |

Construct a Vector3 from the given components.

## Vector3.magnitude(Vector3 v)

```lua
local wishDir = Vector3(0, 0.1, 0);
if (Vector3.magnitude(wishDir) > 0) then
   print("Do stuff")
end
```

`number Vector3.magnitude(Vector3 v)`

| Parameter | Type | Description |
|---|---|---|
| v | Vector3 | Vector3 to find magnitude of. |

Return the magnitude of the given Vector3.

## Vector3.normalize(Vector3 v)

```lua
local wishDir = Vector3(0, 0.1, 0);
wishDir = Vector3.normalize(wishDir);
```

`Vector3 Vector3.normalize(Vector3 v)`

| Parameter | Type | Description |
|---|---|---|
| v | Vector3 | Vector3 to normalize. |

Return a normalized version of the given Vector3.

## Vector3.invert(Vector3 v)

```lua
local vec = Vector3(1, 0, 1);
print(vec); -- {1, 0, 1}
local vec = Vector3.invert(vec);
print(vec); -- {-1, 0, -1}
```

`Vector3 Vector3.invert(Vector3 v)`

| Parameter | Type | Description |
|---|---|---|
| v | Vector3 | Vector3 to invert. |

Return an inverted version of the given Vector3.

## Vector3.dot(Vector3 v1, Vector3 v2)

```lua
local v1 = Vector3(0, 1, 0);
local v2 = Vector3(0, 1, 0);
local dot = Vector3.dot(v1, v2); -- 1 
```

`number Vector3.dot(Vector3 v1, Vector3 v2)`

| Parameter | Type | Description |
|---|---|---|
| v1 | Vector3 | Vector3 to dot product. |
| v2 | Vector3 | Vector3 to dot product. |

Return the dot product of the two given vectors.

## Vector3.cross(Vector3 v1, Vector3 v2)

```lua
local v1 = Vector3(1, 0, 0);
local v2 = Vector3(0, 1, 0);
local cross = Vector3.cross(v1, v2); -- {0, 0, 1}
```

`Vector3 Vector3.cross(Vector3 v1, Vector3 v2)`

| Parameter | Type | Description |
|---|---|---|
| v1 | Vector3 | Vector3 to cross product. |
| v2 | Vector3 | Vector3 to cross product. |

Return the cross product of the two given vectors.

## Vector3.transform(Vector3 v, Matrix4 m)

```lua
local vecTransformed = Vector3.transform(myVec, myMatrix);
```

| Parameter | Type | Description |
|---|---|---|
| v | Vector3 | Vector3 to transform. |
| m | Matrix4 | Matrix4 to transform Vector3 by. |

Return a Vector3 equal to the given Vector3 transformed by the given Matrix4.

## Vector3.unit_x()

```lua
local unitX = Vector3.unit_x() -- {1, 0, 0}
```

`Vector3 Vector3.unit_x()`

Return a Vector3 of magnitude 1 in the x-direction.

## Vector3.unit_y()

```lua
local unitY = Vector3.unit_y() -- {0, 1, 0}
```

`Vector3 Vector3.unit_y()`

Return a Vector3 of magnitude 1 in the y-direction.

## Vector3.unit_z()

```lua
local unitZ = Vector3.unit_z() -- {0, 0, 1}
```

`Vector3 Vector3.unit_z()`

Return a Vector3 of magnitude 1 in the z-direction.

## Vector3:get_x()

```lua
local vec = Vector3(3.14159, 0, 0);
local x = vec:get_x(); -- 3.14159
```

`number Vector3:get_x()`

Return the x component of the given Vector3.

## Vector3:get_y()

```lua
local vec = Vector3(0, 3.14159, 0);
local y = vec:get_y(); -- 3.14159
```

`number Vector3:get_y()`

Return the y component of the given Vector3.

## Vector3:get_z()

```lua
local vec = Vector3(0, 0, 3.14159);
local z = vec:get_z(); -- 3.14159
```

`number Vector3:get_z()`

Return the z component of the given Vector3.

## Vector3:set_x()

```lua
local vec = Vector3(0, 0, 0); -- {0, 0, 0}
vec:set_x(3.14159); -- {3.14159, 0, 0}
```

`Vector3:set_x(number x)`

| Parameter | Type | Description |
|---|---|---|
| x | number | Value to given to x component of given Vector3. |

Set the x component of the given Vector3 to the given value.

## Vector3:set_y()

```lua
local vec = Vector3(0, 0, 0); -- {0, 0, 0}
vec:set_y(3.14159); -- {0, 3.14159, 0}
```

`Vector3:set_y(number y)`

| Parameter | Type | Description |
|---|---|---|
| y | number | Value to given to y component of given Vector3. |

Set the y component of the given Vector3 to the given value.

## Vector3:set_z()

```lua
local vec = Vector3(0, 0, 0); -- {0, 0, 0}
vec:set_z(3.14159); -- {0, 0, 3.14159}
```

`Vector3:set_z(number z)`

| Parameter | Tzpe | Description |
|---|---|---|
| z | number | Value to given to z component of given Vector3. |

Set the z component of the given Vector3 to the given value.

