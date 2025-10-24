##Walls Class
'Walls class. Encapsulates the object that represents walls in Go.'
## Walls class
Encapsulates the object that represents the walls of a 3-D chart.
```go
type Walls struct  {
ptr unsafe.Pointer
}
```
## Constructors
| Method | Description |
| --- | --- |
|[NewWalls](./newwalls/) | Constructs from a parent object. |
## Methods
| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. |
|[GetCenterX](./getcenterx/) | Gets the x coordinate of the left-bottom corner of Wall center in units of 1/4000 of chart's width after calls Chart.Calculate() method. |
|[GetCenterY](./getcentery/) | Gets the y coordinate of the left-bottom corner of Wall center in units of 1/4000 of chart's height after calls Chart.Calculate() method. |
|[GetWidth](./getwidth/) | Gets the width of left to right in units of 1/4000 of chart's width after calls Chart.Calculate() method. |
|[GetDepth](./getdepth/) | Gets the depth front to back in units of 1/4000 of chart's width after calls Chart.Calculate() method. |
|[GetHeight](./getheight/) | Gets the height of top to bottom in units of 1/4000 of chart's height after calls Chart.Calculate() method. |
|[GetCenterXPx](./getcenterxpx/) | Gets the x coordinate of the left-bottom corner of Wall center in units of pixels after calls Chart.Calculate() method. |
|[GetCenterYPx](./getcenterypx/) | Gets the y coordinate of the left-bottom corner of Wall center in units of pixels after calls Chart.Calculate() method. |
|[GetWidthPx](./getwidthpx/) | Gets the width of left to right in units of pixels after calls Chart.Calculate() method. |
|[GetDepthPx](./getdepthpx/) | Gets the depth front to back in units of pixels after calls Chart.Calculate() method. |
|[GetHeightPx](./getheightpx/) | Gets the height of top to bottom in units of pixels after calls Chart.Calculate() method. |
|[GetCubePointCount](./getcubepointcount/) | Gets the number of cube points after calls Chart.Calculate() method. |
|[GetCubePointXPx](./getcubepointxpx/) | Gets x-coordinate of the apex point of walls cube after calls Chart.Calculate() method.The number of apex points of walls cube is eight |
|[GetCubePointYPx](./getcubepointypx/) | Gets y-coordinate of the apex point of walls cube after calls Chart.Calculate() method.The number of apex points of walls cube is eight. |
|[GetBackgroundColor](./getbackgroundcolor/) | Gets or sets the background Color of the Area. |
|[SetBackgroundColor](./setbackgroundcolor/) | Gets or sets the background Color of the Area. |
|[GetForegroundColor](./getforegroundcolor/) | Gets or sets the foreground Color. |
|[SetForegroundColor](./setforegroundcolor/) | Gets or sets the foreground Color. |
|[GetFormatting](./getformatting/) | Represents the formatting of the area. |
|[SetFormatting](./setformatting/) | Represents the formatting of the area. |
|[GetInvertIfNegative](./getinvertifnegative/) | If the property is true and the value of chart point is a negative number,the foreground color and background color will be exchanged. |
|[SetInvertIfNegative](./setinvertifnegative/) | If the property is true and the value of chart point is a negative number,the foreground color and background color will be exchanged. |
|[GetFillFormat](./getfillformat/) | Represents a FillFormat object that contains fill formatting properties for the specified chart or shape. |
|[GetTransparency](./gettransparency/) | Returns or sets the degree of transparency of the area as a value from 0.0 (opaque) through 1.0 (clear). |
|[SetTransparency](./settransparency/) | Returns or sets the degree of transparency of the area as a value from 0.0 (opaque) through 1.0 (clear). |
|[GetBorder](./getborder/) | Gets or sets the border Line. |
|[SetBorder](./setborder/) | Gets or sets the border Line. |
