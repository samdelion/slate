# > Quaternion 

## Quaternion 

```lua
local quat = Quaternion(4, 0.1, 3.0, 1.0);
```

`Quaternion Quaternion(number x, number y, number z, number w)`

| Parameter | Type | Description |
|---|---|---|
| x | number | x component of Quaternion. |
| y | number | y component of Quaternion. |
| z | number | z component of Quaternion. |
| w | number | w component of Quaternion. |

Construct a Quaternion from the given components.

## Quaternion.new(number x, number y, number z, number w)

```lua
local quat = Quaternion.new(4, 0.1, 3.0, 1.0);
```

`Quaternion Quaternion(number x, number y, number z, number w)`

| Parameter | Type | Description |
|---|---|---|
| x | number | x component of Quaternion. |
| y | number | y component of Quaternion. |
| z | number | z component of Quaternion. |
| w | number | w component of Quaternion. |

Construct a Quaternion from the given components.

## Quaternion.create\_from\_axis_angle(Vector3 axis, number angleRadians)

```lua
local axis = Vector3(0, 1, 0);
local angle = math.pi/2.0; 
local quat = Quaternion.create_from_axis_angle(axis, angle);
```

`Quaternion Quaternion.create_from_axis_angle(Vector3 axis, number angleRadians)`

| Parameter | Type | Description |
|---|---|---|
| axis | Vector3 | Axis of Quaternion. |
| angle | number | Angle of Quaternion. |

Return a Quaternion constructed from the given axis and angle.

## Quaternion.magnitude(Quaternion q)

```lua
local quat = Quaternion(1, 0, 0, 0);
print(Quaternion.magnitude(quat)); -- 1
```

`number Quaternion.magnitude(Quaternion q)`

| Parameter | Type | Description |
|---|---|---|
| q | Quaternion | Quaternion to get magnitude of. |

Return the magnitude of the given Quaternion.

## Quaternion.normalize(Quaternion q)

```lua
local quat = Quaternion(2, 0, 0, 0);
print(Quaternion.normalize(quat)); -- {1, 0, 0, 0}
```

`Quaternion Quaternion.normalize(Quaternion q)`

| Parameter | Type | Description |
|---|---|---|
| q | Quaternion | Quaternion to get normalized version of. |

Returns a normalized version of the given Quaternion.

## Quaternion.invert(Quaternion q)

```lua
local quat = Quaternion(2, 0, 0, 0);
print(Quaternion.invert(quat)); -- {-2, 0, 0, 0}
```

`Quaternion Quaternion.invert(Quaternion q)`

| Parameter | Type | Description |
|---|---|---|
| q | Quaternion | Quaternion to get inverted version of. |

Returns an inverted version of the given Quaternion.

## Quaternion.dot(Quaternion q1, Quaternion q2)

```lua
local q1 = Quaternion(1, 0, 0, 0);
local q2 = Quaternion(1, 0, 0, 0);
local number = Quaternion.dot(q1, q2);
```

`number Quaternion.dot(Quaternion q1, Quaternion q2)`

| Parameter | Type | Description |
|---|---|---|
| q1 | Quaternion | Quaternion get dot product of. |
| q2 | Quaternion | Quaternion get dot product of. |

Returns the dot product of the two given Quaternions.
