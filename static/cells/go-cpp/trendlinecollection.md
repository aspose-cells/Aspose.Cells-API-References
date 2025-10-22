##TrendlineCollection Class
'TrendlineCollection class. Encapsulates the object that represents trendlinecollection in Go.'
## TrendlineCollection class
Represents a collection of all the <see cref="Trendline"/> objects for the specified data series.
```go
type TrendlineCollection struct  {
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
|[Add_TrendlineType](./add_trendlinetype/) | Adds a Trendline object to this collection with specified type. |
|[Add_TrendlineType_String](./add_trendlinetype_string/) | Adds a Trendline object to this collection with specified type and name. |
|[Get](./get/) | Gets a Trendline object by its index. |
|[GetCount](./getcount/) |  |
