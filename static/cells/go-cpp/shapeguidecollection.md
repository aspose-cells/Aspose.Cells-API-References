##ShapeGuideCollection Class
'ShapeGuideCollection class. Encapsulates the object that represents shapeguidecollection in Go.'
## ShapeGuideCollection class
Encapsulates a collection of shape guide
```go
type ShapeGuideCollection struct  {
ptr unsafe.Pointer
}
```
## Constructors
| Method | Description |
| --- | --- |
|[NewShapeGuideCollection](./newshapeguidecollection/) | Default constructor. |
## Methods
| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. |
|[Add](./add/) | Adds a shape guide.(Important: This feature is currently only available for Excel07 and above) |
|[Get](./get/) | Gets a shape guide by index |
|[GetCount](./getcount/) |  |
