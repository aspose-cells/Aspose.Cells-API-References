##PlotArea Class
'PlotArea class. Encapsulates the object that represents plotarea in Go.'
## PlotArea class
Encapsulates the object that represents the plot area in a chart.
```go
type PlotArea struct  {
ptr unsafe.Pointer
}
```
## Constructors
| Method | Description |
| --- | --- |
|[NewPlotArea](./newplotarea/) | Constructs from a parent object. |
## Methods
| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. |
|[GetXRatioToChart](./getxratiotochart/) | Gets or gets the x coordinate of the upper left corner of plot-area bounding box in units of ratio of the chart area. |
|[SetXRatioToChart](./setxratiotochart/) | Gets or gets the x coordinate of the upper left corner of plot-area bounding box in units of ratio of the chart area. |
|[GetYRatioToChart](./getyratiotochart/) | Gets or gets the y coordinate of the upper top corner  of plot-area bounding box in units of ratio of the chart area. |
|[SetYRatioToChart](./setyratiotochart/) | Gets or gets the y coordinate of the upper top corner  of plot-area bounding box in units of ratio of the chart area. |
|[GetHeightRatioToChart](./getheightratiotochart/) | Gets or sets the height of plot-area bounding box in units of ratio of the chart area. |
|[SetHeightRatioToChart](./setheightratiotochart/) | Gets or sets the height of plot-area bounding box in units of ratio of the chart area. |
|[GetWidthRatioToChart](./getwidthratiotochart/) | Gets or sets the width of plot-area bounding box in units of ratio of the chart area. |
|[SetWidthRatioToChart](./setwidthratiotochart/) | Gets or sets the width of plot-area bounding box in units of ratio of the chart area. |
|[GetInnerXRatioToChart](./getinnerxratiotochart/) | Gets or gets the x coordinate of the upper top corner of plot area in units of ratio of the chart area. |
|[SetInnerXRatioToChart](./setinnerxratiotochart/) | Gets or gets the x coordinate of the upper top corner of plot area in units of ratio of the chart area. |
|[GetInnerYRatioToChart](./getinneryratiotochart/) | Gets or gets the x coordinate of the upper top corner of plot area in units of ratio of the chart area. |
|[SetInnerYRatioToChart](./setinneryratiotochart/) | Gets or gets the x coordinate of the upper top corner of plot area in units of ratio of the chart area. |
|[GetInnerHeightRatioToChart](./getinnerheightratiotochart/) | Gets or sets the height of plot area in units of ratio of the chart area. |
|[SetInnerHeightRatioToChart](./setinnerheightratiotochart/) | Gets or sets the height of plot area in units of ratio of the chart area. |
|[GetInnerWidthRatioToChart](./getinnerwidthratiotochart/) | Gets or sets the width  of plot area in units of ratio of the chart area. |
|[SetInnerWidthRatioToChart](./setinnerwidthratiotochart/) | Gets or sets the width  of plot area in units of ratio of the chart area. |
|[SetPositionAuto](./setpositionauto/) | Set position of the plot area to automatic |
|[IsAutomaticSize](./isautomaticsize/) | Indicates whether the plot area is automatic sized. |
|[SetIsAutomaticSize](./setisautomaticsize/) | Indicates whether the plot area is automatic sized. |
|[IsInnerMode](./isinnermode/) | Indicates whether the size of the plot area size includes the tick marks, and the axis labels.False specifies that the size shall determine the size of the plot area, the tick marks, and the axis labels. |
|[SetIsInnerMode](./setisinnermode/) | Indicates whether the size of the plot area size includes the tick marks, and the axis labels.False specifies that the size shall determine the size of the plot area, the tick marks, and the axis labels. |
|[GetBackgroundMode](./getbackgroundmode/) | Gets and sets the display mode of the background |
|[SetBackgroundMode](./setbackgroundmode/) | Gets and sets the display mode of the background |
|[GetShadow](./getshadow/) | True if the frame has a shadow. |
|[SetShadow](./setshadow/) | True if the frame has a shadow. |
|[GetShapeProperties](./getshapeproperties/) | Gets the ShapeProperties object. |
|[IsDefaultPosBeSet](./isdefaultposbeset/) | Indicates whether default position(DefaultX, DefaultY, DefaultWidth and DefaultHeight) are set. |
|[GetDefaultXRatioToChart](./getdefaultxratiotochart/) | Represents x of default position in units of Fraction of the chart area. |
|[GetDefaultYRatioToChart](./getdefaultyratiotochart/) | Represents y of default position in units of Fraction of the chart area. |
|[GetDefaultWidthRatioToChart](./getdefaultwidthratiotochart/) | Represents width of default position in units of Fraction of the chart area. |
|[GetDefaultHeightRatioToChart](./getdefaultheightratiotochart/) | Represents height of default position in units of Fraction of the chart area. |
|[GetBorder](./getborder/) | Gets the Line</see>. |
|[GetArea](./getarea/) | Gets the Area</see>. |
|[GetTextOptions](./gettextoptions/) | Gets and sets the options of the text. |
|[GetFont](./getfont/) | Gets a Font object of the specified ChartFrame object. |
|[GetAutoScaleFont](./getautoscalefont/) | True if the text in the object changes font size when the object size changes. The default value is True. |
|[SetAutoScaleFont](./setautoscalefont/) | True if the text in the object changes font size when the object size changes. The default value is True. |
|[GetXPixel](./getxpixel/) | Gets or sets the x coordinate of the upper left corner in units of Pixel. |
|[SetXPixel](./setxpixel/) | Gets or sets the x coordinate of the upper left corner in units of Pixel. |
|[GetYPixel](./getypixel/) | Gets or sets the y coordinate of the upper left corner in units of Pixel. |
|[SetYPixel](./setypixel/) | Gets or sets the y coordinate of the upper left corner in units of Pixel. |
|[GetWidthPixel](./getwidthpixel/) | Gets or sets the width of frame in units of Pixel. |
|[SetWidthPixel](./setwidthpixel/) | Gets or sets the width of frame in units of Pixel. |
|[GetHeightPixel](./getheightpixel/) | Gets or sets the height of frame in units of Pixel. |
|[SetHeightPixel](./setheightpixel/) | Gets or sets the height of frame in units of Pixel. |
