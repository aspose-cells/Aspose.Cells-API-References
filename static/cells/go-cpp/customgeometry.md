##CustomGeometry Class
'CustomGeometry class. Encapsulates the object that represents customgeometry in Go.'
## CustomGeometry class
Represents a custom geometric shape.
```go
type CustomGeometry struct  {
ptr unsafe.Pointer
}
```
## Constructors
| Method | Description |
| --- | --- |
|[NewCustomGeometry](./newcustomgeometry/) | Constructs from a parent object. |
## Methods
| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. |
|[GetPaths](./getpaths/) | Gets path collection information when shape is a NotPrimitive autoshape |
|[GetShapeAdjustValues](./getshapeadjustvalues/) | Gets a collection of shape adjust value |
