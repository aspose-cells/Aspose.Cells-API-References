##ChartPointCollection Class
'ChartPointCollection class. Encapsulates the object that represents chartpointcollection in Go.'
## ChartPointCollection class
Represents a collection that contains all the points in one series.
```go
type ChartPointCollection struct  {
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
|[GetEnumerator](./getenumerator/) | Returns an enumerator for the entire ChartPointCollection. |
|[Clear](./clear/) | Remove all setting of the chart points. |
|[RemoveAt](./removeat/) | Removes point at the index of the series.. |
|[GetCount](./getcount/) | Gets the count of the chart point. |
|[Get](./get/) | Gets the ChartPoint element at the specified index in the series. |
