##ChartArea Class
'ChartArea class. Encapsulates the object that represents chartarea in Go.'
## ChartArea class
Encapsulates the object that represents the chart area in the worksheet.
```go
type ChartArea struct  {
ptr unsafe.Pointer
}
```
## Constructors
| Method | Description |
| --- | --- |
|[NewChartArea](./newchartarea/) | Constructs from a parent object. |
## Methods
| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. |
|[GetXRatioToChart](./getxratiotochart/) | Gets or gets the horizontal offset from its upper left corner column, in units of ratio of the chart area. |
|[SetXRatioToChart](./setxratiotochart/) | Gets or gets the horizontal offset from its upper left corner column, in units of ratio of the chart area. |
|[GetYRatioToChart](./getyratiotochart/) | Gets or gets the vertical offset from its upper left corner row, in units of ratio of the chart area. |
|[SetYRatioToChart](./setyratiotochart/) | Gets or gets the vertical offset from its upper left corner row, in units of ratio of the chart area. |
|[GetHeightRatioToChart](./getheightratiotochart/) | Gets or sets the vertical offset from its lower right corner row, in units of ratio of the chart area. |
|[SetHeightRatioToChart](./setheightratiotochart/) | Gets or sets the vertical offset from its lower right corner row, in units of ratio of the chart area. |
|[GetWidthRatioToChart](./getwidthratiotochart/) | Gets or sets the horizontal offset from its lower right corner column, in units of ratio of the chart area. |
|[SetWidthRatioToChart](./setwidthratiotochart/) | Gets or sets the horizontal offset from its lower right corner column, in units of ratio of the chart area. |
|[GetFont](./getfont/) | Gets a Font object of the specified chartarea object. |
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
|[GetAutoScaleFont](./getautoscalefont/) | True if the text in the object changes font size when the object size changes. The default value is True. |
|[SetAutoScaleFont](./setautoscalefont/) | True if the text in the object changes font size when the object size changes. The default value is True. |
|[IsAutomaticSize](./isautomaticsize/) | Indicates whether the chart frame is automatic sized. |
|[SetIsAutomaticSize](./setisautomaticsize/) | Indicates whether the chart frame is automatic sized. |
|[GetXPixel](./getxpixel/) | Gets or sets the x coordinate of the upper left corner in units of Pixel. |
|[SetXPixel](./setxpixel/) | Gets or sets the x coordinate of the upper left corner in units of Pixel. |
|[GetYPixel](./getypixel/) | Gets or sets the y coordinate of the upper left corner in units of Pixel. |
|[SetYPixel](./setypixel/) | Gets or sets the y coordinate of the upper left corner in units of Pixel. |
|[GetWidthPixel](./getwidthpixel/) | Gets or sets the width of frame in units of Pixel. |
|[SetWidthPixel](./setwidthpixel/) | Gets or sets the width of frame in units of Pixel. |
|[GetHeightPixel](./getheightpixel/) | Gets or sets the height of frame in units of Pixel. |
|[SetHeightPixel](./setheightpixel/) | Gets or sets the height of frame in units of Pixel. |
|[SetPositionAuto](./setpositionauto/) | Set position of the frame to automatic |
