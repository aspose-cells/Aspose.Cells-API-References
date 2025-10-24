##Bevel Class
'Bevel class. Encapsulates the object that represents bevel in Go.'
## Bevel class
Represents a bevel of a shape
```go
type Bevel struct  {
ptr unsafe.Pointer
}
```
## Constructors
| Method | Description |
| --- | --- |
## Methods
| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. |
|[GetWidth](./getwidth/) | Gets and sets the width of the bevel, or how far into the shape it is applied.In unit of Points. |
|[SetWidth](./setwidth/) | Gets and sets the width of the bevel, or how far into the shape it is applied.In unit of Points. |
|[GetHeight](./getheight/) | Gets and sets the height of the bevel, or how far above the shape it is applied.In unit of Points. |
|[SetHeight](./setheight/) | Gets and sets the height of the bevel, or how far above the shape it is applied.In unit of Points. |
|[GetType](./gettype/) | Gets and sets the preset bevel type. |
|[SetType](./settype/) | Gets and sets the preset bevel type. |
