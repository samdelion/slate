# > Matrix4 

## Matrix4 

```lua
local mat = Matrix4(1.0); -- identity matrix
```

`Matrix4 Matrix4(number leading)`

| Parameter | Type | Description |
|---|---|---|
| leading | number | Number to have along leading diagonal of Matrix4. |

Construct a diagonal Matrix4 with the leading edge filled with the given number.

## Matrix4.create\_translation_matrix(Vector3 translation)

```lua
local translationMatrix = Matrix4.create_translation_matrix(Vector3(0, 3, -10));
```

`Matrix4 Matrix4.create_translation_matrix(Vector3 translation)`

| Parameter | Type | Description |
|---|---|---|
| translation | Vector3 | Translation to get. |

Create a Matrix4 representing a translation transformation.

## Matrix4.create\_scale_matrix(Vector3 scale)

```lua
local scaleMatrix = Matrix4.create_scale_matrix(Vector3(0.1, 0.1, 0.1));
```

`Matrix4 Matrix4.create_scale_matrix(Vector3 scale)`

| Parameter | Type | Description |
|---|---|---|
| scale | Vector3 | Scale to get. |

Create a Matrix4 representing a scale transformation.

## Matrix4.create\_from_quaternion(Quaternion rotation)

```lua
local myQuat = Quaternion.create_from_axis_angle(Vector3(0, 1, 0), math.pi/2.0);
local rotation = Matrix4.create_from_quaternion(myQuat);
```

`Matrix4 Matrix4.create_from_quaternion(Quaternion rotation)`

| Parameter | Type | Description |
|---|---|---|
| rotation | Quaternion | Rotation to get. |

Create a Matrix4 representing a rotation transformation.

## Matrix4.transpose(Matrix4 mat)

```lua
local mat = Matrix4(1.0); -- identity matrix
local mat = Matrix4.transpose(mat); -- identity matrix
```

`Matrix4 Matrix4.transpose(Matrix4 mat)`

| Parameter | Type | Description |
|---|---|---|
| mat | Matrix4 | Matrix4 to transpose. |

Returns a transposed (swapped rows and columns) version of the given Matrix4.

## Matrix4.inverse(Matrix4 mat)

```lua
local mat = Matrix4(1.0); -- identity matrix
local mat = Matrix4.inverse(mat); -- identity matrix
```

`Matrix4 Matrix4.inverse(Matrix4 mat)`

| Parameter | Type | Description |
|---|---|---|
| mat | Matrix4 | Matrix4 to return inverse of. |

Returns a matrix-inversed version of the given Matrix4.
