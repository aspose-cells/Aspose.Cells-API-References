##ChartDataTable Class
'ChartDataTable class. Encapsulates the object that represents chartdatatable in Go.'
## ChartDataTable class
Represents a chart data table.
```go
type ChartDataTable struct  {
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
|[GetFont](./getfont/) | Gets a Font object which represents the font setting of the specified chart data table. |
|[GetAutoScaleFont](./getautoscalefont/) | True if the text in the object changes font size when the object size changes.The default value is True. |
|[SetAutoScaleFont](./setautoscalefont/) | True if the text in the object changes font size when the object size changes.The default value is True. |
|[GetBackgroundMode](./getbackgroundmode/) | Gets and sets the display mode of the background |
|[SetBackgroundMode](./setbackgroundmode/) | Gets and sets the display mode of the background |
|[GetHasHorizontalBorder](./gethashorizontalborder/) | True if the chart data table has horizontal cell borders |
|[SetHasHorizontalBorder](./sethashorizontalborder/) | True if the chart data table has horizontal cell borders |
|[GetHasVerticalBorder](./gethasverticalborder/) | True if the chart data table has vertical cell borders |
|[SetHasVerticalBorder](./sethasverticalborder/) | True if the chart data table has vertical cell borders |
|[GetHasOutlineBorder](./gethasoutlineborder/) | True if the chart data table has outline borders |
|[SetHasOutlineBorder](./sethasoutlineborder/) | True if the chart data table has outline borders |
|[GetShowLegendKey](./getshowlegendkey/) | True if the data label legend key is visible. |
|[SetShowLegendKey](./setshowlegendkey/) | True if the data label legend key is visible. |
|[GetBorder](./getborder/) | Returns a Border object that represents the border of the object |
