##Class DataLabels
Aspose.Cells.Charts.DataLabels class. Encapsulates a collection of all the DataLabel objects for the specified Series
## DataLabels class
Encapsulates a collection of all the DataLabel objects for the specified Series.
```csharp
public class DataLabels : ChartTextFrame
```
## Properties
| Name | Description |
| --- | --- |
| override [Area](../../aspose.cells.charts/datalabels/area/) { get; } | Gets the [`area`](./area/). |
| virtual [AutoScaleFont](../../aspose.cells.charts/chartframe/autoscalefont/) { get; set; } | True if the text in the object changes font size when the object size changes. The default value is True.(Inherited from [`ChartFrame`](../chartframe/).) |
| [Background](../../aspose.cells.charts/chartframe/background/) { get; set; } | (**Obsolete.**) Gets and sets the display mode of the background(Inherited from [`ChartFrame`](../chartframe/).) |
| [BackgroundMode](../../aspose.cells.charts/datalabels/backgroundmode/) { get; set; } | Gets and sets the display mode of the background |
| override [Border](../../aspose.cells.charts/datalabels/border/) { get; } | Gets the [`border`](../../aspose.cells.drawing/line/). |
| [DefaultHeight](../../aspose.cells.charts/chartframe/defaultheight/) { get; } | (**Obsolete.**) Represents height of default position in units of 1/4000 of the chart area.(Inherited from [`ChartFrame`](../chartframe/).) |
| [DefaultHeightRatioToChart](../../aspose.cells.charts/chartframe/defaultheightratiotochart/) { get; } | Represents height of default position in units of Fraction of the chart area.(Inherited from [`ChartFrame`](../chartframe/).) |
| [DefaultWidth](../../aspose.cells.charts/chartframe/defaultwidth/) { get; } | (**Obsolete.**) Represents width of default position in units of 1/4000 of the chart area.(Inherited from [`ChartFrame`](../chartframe/).) |
| [DefaultWidthRatioToChart](../../aspose.cells.charts/chartframe/defaultwidthratiotochart/) { get; } | Represents width of default position in units of Fraction of the chart area.(Inherited from [`ChartFrame`](../chartframe/).) |
| [DefaultX](../../aspose.cells.charts/chartframe/defaultx/) { get; } | (**Obsolete.**) Represents x of default position in units of 1/4000 of the chart area.(Inherited from [`ChartFrame`](../chartframe/).) |
| [DefaultXRatioToChart](../../aspose.cells.charts/chartframe/defaultxratiotochart/) { get; } | Represents x of default position in units of Fraction of the chart area.(Inherited from [`ChartFrame`](../chartframe/).) |
| [DefaultY](../../aspose.cells.charts/chartframe/defaulty/) { get; } | (**Obsolete.**) Represents y of default position in units of 1/4000 of the chart area.(Inherited from [`ChartFrame`](../chartframe/).) |
| [DefaultYRatioToChart](../../aspose.cells.charts/chartframe/defaultyratiotochart/) { get; } | Represents y of default position in units of Fraction of the chart area.(Inherited from [`ChartFrame`](../chartframe/).) |
| override [DirectionType](../../aspose.cells.charts/datalabels/directiontype/) { get; set; } | Gets and sets the direction of text. |
| override [Font](../../aspose.cells.charts/datalabels/font/) { get; } | Gets the font of the DataLabels; |
| virtual [Height](../../aspose.cells.charts/chartframe/height/) { get; set; } | (**Obsolete.**) Gets or sets the height of frame in units of 1/4000 of the chart area.(Inherited from [`ChartFrame`](../chartframe/).) |
| virtual [HeightPixel](../../aspose.cells.charts/chartframe/heightpixel/) { get; set; } | Gets or sets the height of frame in units of Pixel.(Inherited from [`ChartFrame`](../chartframe/).) |
| virtual [HeightRatioToChart](../../aspose.cells.charts/chartframe/heightratiotochart/) { get; set; } | Gets or sets the height of frame in units of ratio of the chart area.(Inherited from [`ChartFrame`](../chartframe/).) |
| [IsAutomaticRotation](../../aspose.cells.charts/charttextframe/isautomaticrotation/) { get; } | Indicates whether the text of the chart is automatically rotated.(Inherited from [`ChartTextFrame`](../charttextframe/).) |
| virtual [IsAutomaticSize](../../aspose.cells.charts/chartframe/isautomaticsize/) { get; set; } | Indicates whether the chart frame is automatic sized.(Inherited from [`ChartFrame`](../chartframe/).) |
| override [IsAutoText](../../aspose.cells.charts/datalabels/isautotext/) { get; set; } | Indicates the text is auto generated. |
| [IsDefaultPosBeSet](../../aspose.cells.charts/chartframe/isdefaultposbeset/) { get; } | Indicates whether default position(DefaultX, DefaultY, DefaultWidth and DefaultHeight) are set.(Inherited from [`ChartFrame`](../chartframe/).) |
| [IsDeleted](../../aspose.cells.charts/charttextframe/isdeleted/) { get; set; } | Indicates whether this data labels is deleted.(Inherited from [`ChartTextFrame`](../charttextframe/).) |
| [IsInnerMode](../../aspose.cells.charts/chartframe/isinnermode/) { get; set; } | Indicates whether the size of the plot area size includes the tick marks, and the axis labels. False specifies that the size shall determine the size of the plot area, the tick marks, and the axis labels.(Inherited from [`ChartFrame`](../chartframe/).) |
| [IsNeverOverlap](../../aspose.cells.charts/datalabels/isneveroverlap/) { get; set; } | Indicates whether the datalabels display never overlap. (For Pie chart) |
| [IsResizeShapeToFitText](../../aspose.cells.charts/charttextframe/isresizeshapetofittext/) { get; set; } | Gets or sets whether a shape should be auto-fit to fully contain the text described within it. Auto-fitting is when text within a shape is scaled in order to contain all the text inside.(Inherited from [`ChartTextFrame`](../charttextframe/).) |
| override [IsTextWrapped](../../aspose.cells.charts/datalabels/istextwrapped/) { get; set; } | Gets or sets a value indicating whether the text is wrapped. |
| virtual [LinkedSource](../../aspose.cells.charts/charttextframe/linkedsource/) { get; set; } | Gets and sets a reference to the worksheet.(Inherited from [`ChartTextFrame`](../charttextframe/).) |
| [Number](../../aspose.cells.charts/datalabels/number/) { get; set; } | Gets and sets the built-in number format. |
| [NumberFormat](../../aspose.cells.charts/datalabels/numberformat/) { get; set; } | Represents the format string for the DataLabels object. |
| [NumberFormatLinked](../../aspose.cells.charts/datalabels/numberformatlinked/) { get; set; } | True if the number format is linked to the cells (so that the number format changes in the labels when it changes in the cells). |
| [Position](../../aspose.cells.charts/datalabels/position/) { get; set; } | Represents the position of the data label. |
| [ReadingOrder](../../aspose.cells.charts/charttextframe/readingorder/) { get; set; } | Represents text reading order.(Inherited from [`ChartTextFrame`](../charttextframe/).) |
| [RotationAngle](../../aspose.cells.charts/charttextframe/rotationangle/) { get; set; } | Represents text rotation angle.(Inherited from [`ChartTextFrame`](../charttextframe/).) |
| [SeparatorType](../../aspose.cells.charts/datalabels/separatortype/) { get; set; } | Gets or sets the separator type used for the data labels on a chart. |
| [SeparatorValue](../../aspose.cells.charts/datalabels/separatorvalue/) { get; set; } | Gets or sets the separator value used for the data labels on a chart. |
| [Shadow](../../aspose.cells.charts/chartframe/shadow/) { get; set; } | True if the frame has a shadow.(Inherited from [`ChartFrame`](../chartframe/).) |
| [ShapeProperties](../../aspose.cells.charts/chartframe/shapeproperties/) { get; } | Gets the [`ShapeProperties`](../chartframe/shapeproperties/) object.(Inherited from [`ChartFrame`](../chartframe/).) |
| [ShapeType](../../aspose.cells.charts/datalabels/shapetype/) { get; set; } | Gets or sets shape type of data label. |
| [ShowBubbleSize](../../aspose.cells.charts/datalabels/showbubblesize/) { get; set; } | Represents a specified chart's data label percentage value display behavior. True displays the percentage value. False to hide. |
| [ShowCategoryName](../../aspose.cells.charts/datalabels/showcategoryname/) { get; set; } | Represents a specified chart's data label category name display behavior.True to display the category name for the data labels on a chart. False to hide. |
| [ShowCellRange](../../aspose.cells.charts/datalabels/showcellrange/) { get; set; } | Indicates whether showing cell range as the data labels. |
| [ShowLegendKey](../../aspose.cells.charts/datalabels/showlegendkey/) { get; set; } | Represents a specified chart's data label legend key display behavior. True if the data label legend key is visible. |
| [ShowPercentage](../../aspose.cells.charts/datalabels/showpercentage/) { get; set; } | Represents a specified chart's data label percentage value display behavior. True displays the percentage value. False to hide. |
| [ShowSeriesName](../../aspose.cells.charts/datalabels/showseriesname/) { get; set; } | Indicates whether the series name displays for the data labels on a chart. True to show the series name. False to hide. |
| [ShowValue](../../aspose.cells.charts/datalabels/showvalue/) { get; set; } | Represents a specified chart's data label values display behavior. True displays the values. False to hide. |
| override [Text](../../aspose.cells.charts/datalabels/text/) { get; set; } | Gets or sets the text of data label. |
| [TextDirection](../../aspose.cells.charts/charttextframe/textdirection/) { get; set; } | (**Obsolete.**) Represents text reading order.(Inherited from [`ChartTextFrame`](../charttextframe/).) |
| virtual [TextFont](../../aspose.cells.charts/chartframe/textfont/) { get; } | (**Obsolete.**) Gets a [`Font`](../chartframe/font/) object of the specified ChartFrame object.(Inherited from [`ChartFrame`](../chartframe/).) |
| [TextHorizontalAlignment](../../aspose.cells.charts/charttextframe/texthorizontalalignment/) { get; set; } | Gets and sets the text horizontal alignment.(Inherited from [`ChartTextFrame`](../charttextframe/).) |
| virtual [TextOptions](../../aspose.cells.charts/chartframe/textoptions/) { get; } | Gets and sets the options of the text.(Inherited from [`ChartFrame`](../chartframe/).) |
| [TextVerticalAlignment](../../aspose.cells.charts/charttextframe/textverticalalignment/) { get; set; } | Gets or sets the text vertical alignment of text.(Inherited from [`ChartTextFrame`](../charttextframe/).) |
| virtual [Width](../../aspose.cells.charts/chartframe/width/) { get; set; } | (**Obsolete.**) Gets or sets the width of frame in units of 1/4000 of the chart area.(Inherited from [`ChartFrame`](../chartframe/).) |
| virtual [WidthPixel](../../aspose.cells.charts/chartframe/widthpixel/) { get; set; } | Gets or sets the width of frame in units of Pixel.(Inherited from [`ChartFrame`](../chartframe/).) |
| virtual [WidthRatioToChart](../../aspose.cells.charts/chartframe/widthratiotochart/) { get; set; } | Gets or sets the width of frame in units of ratio of the chart area.(Inherited from [`ChartFrame`](../chartframe/).) |
| virtual [X](../../aspose.cells.charts/chartframe/x/) { get; set; } | (**Obsolete.**) Gets or sets the x coordinate of the upper left corner in units of 1/4000 of the chart area.(Inherited from [`ChartFrame`](../chartframe/).) |
| virtual [XPixel](../../aspose.cells.charts/chartframe/xpixel/) { get; set; } | Gets or sets the x coordinate of the upper left corner in units of Pixel.(Inherited from [`ChartFrame`](../chartframe/).) |
| virtual [XRatioToChart](../../aspose.cells.charts/chartframe/xratiotochart/) { get; set; } | Gets or sets the x coordinate of the upper left corner in units of ratio of the chart area.(Inherited from [`ChartFrame`](../chartframe/).) |
| virtual [Y](../../aspose.cells.charts/chartframe/y/) { get; set; } | (**Obsolete.**) Gets or sets the y coordinate of the upper left corner in units of 1/4000 of the chart area.(Inherited from [`ChartFrame`](../chartframe/).) |
| virtual [YPixel](../../aspose.cells.charts/chartframe/ypixel/) { get; set; } | Gets or sets the y coordinate of the upper left corner in units of Pixel.(Inherited from [`ChartFrame`](../chartframe/).) |
| virtual [YRatioToChart](../../aspose.cells.charts/chartframe/yratiotochart/) { get; set; } | Gets or sets the y coordinate of the upper left corner in units of ratio of the chart area.(Inherited from [`ChartFrame`](../chartframe/).) |
## Methods
| Name | Description |
| --- | --- |
| [ApplyFont](../../aspose.cells.charts/datalabels/applyfont/)() | Apply the font of the datalabels to all child nodes. |
| [Characters](../../aspose.cells.charts/charttextframe/characters/)(int, int) | Returns a Characters object that represents a range of characters within the text.(Inherited from [`ChartTextFrame`](../charttextframe/).) |
| virtual [SetPositionAuto](../../aspose.cells.charts/chartframe/setpositionauto/)() | Set position of the frame to automatic(Inherited from [`ChartFrame`](../chartframe/).) |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Charts;
using System;
public class DataLabelsDemo
{
public static void DataLabelsExample()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue("Category");
worksheet.Cells["A2"].PutValue("A");
worksheet.Cells["A3"].PutValue("B");
worksheet.Cells["A4"].PutValue("C");
worksheet.Cells["B1"].PutValue("Value");
worksheet.Cells["B2"].PutValue(10);
worksheet.Cells["B3"].PutValue(20);
worksheet.Cells["B4"].PutValue(30);
// Add a chart to the worksheet
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
Chart chart = worksheet.Charts[chartIndex];
// Add series to the chart
chart.NSeries.Add("B2:B4", true);
chart.NSeries.CategoryData = "A2:A4";
// Access the DataLabels of the first series
DataLabels dataLabels = chart.NSeries[0].DataLabels;
// Set properties of DataLabels
dataLabels.Position = LabelPositionType.InsideBase;
dataLabels.ShowCategoryName = true;
dataLabels.ShowValue = true;
dataLabels.ShowPercentage = false;
dataLabels.ShowLegendKey = false;
dataLabels.IsAutoText = true;
dataLabels.DirectionType = ChartTextDirectionType.Horizontal;
dataLabels.Text = "Custom Text";
dataLabels.IsTextWrapped = true;
dataLabels.BackgroundMode = BackgroundMode.Transparent;
dataLabels.ShowCellRange = false;
dataLabels.ShowBubbleSize = false;
dataLabels.ShowSeriesName = false;
dataLabels.NumberFormat = "0.00";
dataLabels.Number = 0;
dataLabels.NumberFormatLinked = false;
dataLabels.SeparatorType = DataLabelsSeparatorType.Comma;
dataLabels.SeparatorValue = ", ";
dataLabels.IsNeverOverlap = true;
dataLabels.IsDeleted = false;
dataLabels.TextHorizontalAlignment = TextAlignmentType.Center;
dataLabels.TextVerticalAlignment = TextAlignmentType.Center;
dataLabels.RotationAngle = 0;
dataLabels.LinkedSource = "";
dataLabels.TextDirection = TextDirectionType.LeftToRight;
dataLabels.ReadingOrder = TextDirectionType.LeftToRight;
dataLabels.IsResizeShapeToFitText = true;
dataLabels.IsInnerMode = false;
dataLabels.AutoScaleFont = true;
dataLabels.Background = BackgroundMode.Transparent;
dataLabels.IsAutomaticSize = true;
dataLabels.X = 0;
dataLabels.Y = 0;
dataLabels.Height = 100;
dataLabels.Width = 100;
dataLabels.Shadow = false;
// Save the workbook
workbook.Save("DataLabelsExample.xlsx");
workbook.Save("DataLabelsExample.pdf");
}
}
}
```
### See Also
* class [ChartTextFrame](../charttextframe/)
* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)
