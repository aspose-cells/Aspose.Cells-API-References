##SeriesCollection Class
'SeriesCollection class. Encapsulates the object that represents seriescollection in Go.'
## SeriesCollection class
Encapsulates a collection of <see cref="Series"/> objects.
```go
type SeriesCollection struct  {
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
|[Get](./get/) | Gets the Series element at the specified index. |
|[GetSeriesByOrder](./getseriesbyorder/) | Gets the Series element by order. |
|[RemoveAt](./removeat/) | Remove at a series at the specific index. |
|[GetCategoryData](./getcategorydata/) | Gets or sets the range of category Axis values.It can be a range of cells (such as, "d1:e10"),or a sequence of values (such as,"{2,6,8,10}"). |
|[SetCategoryData](./setcategorydata/) | Gets or sets the range of category Axis values.It can be a range of cells (such as, "d1:e10"),or a sequence of values (such as,"{2,6,8,10}"). |
|[GetSecondCategoryData](./getsecondcategorydata/) | Gets or sets the range of second category Axis values.It can be a range of cells (such as, "d1:e10"),or a sequence of values (such as,"{2,6,8,10}").Only effects when some ASerieses plot on the second axis. |
|[SetSecondCategoryData](./setsecondcategorydata/) | Gets or sets the range of second category Axis values.It can be a range of cells (such as, "d1:e10"),or a sequence of values (such as,"{2,6,8,10}").Only effects when some ASerieses plot on the second axis. |
|[SwapSeries](./swapseries/) | Directly changes the orders of the two series. |
|[SetSeriesNames](./setseriesnames/) | Sets the name of all the serieses in the chart. |
|[AddR1C1](./addr1c1/) | Adds the Series collection to a chart. |
|[Add_String_Bool](./add_string_bool/) | Adds the Series collection to a chart. |
|[Add_String_Bool_Bool](./add_string_bool_bool/) | Adds the Series collection to a chart. |
|[IsColorVaried](./iscolorvaried/) | Represents if the color of points is varied. |
|[SetIsColorVaried](./setiscolorvaried/) | Represents if the color of points is varied. |
|[Clear](./clear/) | Clears the collection |
|[ChangeColors](./changecolors/) | Set Monochromatic Palette for chart series. |
|[GetCount](./getcount/) |  |
