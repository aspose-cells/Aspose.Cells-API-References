##ColorFilter Class
'ColorFilter class. Encapsulates the object that represents colorfilter in Go.'
## ColorFilter class
Represents filtering the range by color.
```go
type ColorFilter struct  {
ptr unsafe.Pointer
}
```
## Constructors
| Method | Description |
| --- | --- |
|[NewColorFilter](./newcolorfilter/) | Constructs from an Object convertible to this. |
## Methods
| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. |
|[ToObject](./toobject/) | Gets the Object. |
|[GetFilterByFillColor](./getfilterbyfillcolor/) | Whether filter by the cell's fill color. |
|[SetFilterByFillColor](./setfilterbyfillcolor/) | Whether filter by the cell's fill color. |
|[GetColor](./getcolor/) | Gets the color of this filter. |
