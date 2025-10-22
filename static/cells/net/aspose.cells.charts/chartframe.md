##Class ChartFrame
Aspose.Cells.Charts.ChartFrame class. Encapsulates the object that represents the frame object in a chart
## ChartFrame class
Encapsulates the object that represents the frame object in a chart.
```csharp
public class ChartFrame
```
## Properties
| Name | Description |
| --- | --- |
| virtual [Area](../../aspose.cells.charts/chartframe/area/) { get; } | Gets the [`area`](./area/). |
| virtual [AutoScaleFont](../../aspose.cells.charts/chartframe/autoscalefont/) { get; set; } | True if the text in the object changes font size when the object size changes. The default value is True. |
| [Background](../../aspose.cells.charts/chartframe/background/) { get; set; } | (**Obsolete.**) Gets and sets the display mode of the background |
| [BackgroundMode](../../aspose.cells.charts/chartframe/backgroundmode/) { get; set; } | Gets and sets the display mode of the background |
| virtual [Border](../../aspose.cells.charts/chartframe/border/) { get; } | Gets the [`border`](../../aspose.cells.drawing/line/). |
| [DefaultHeight](../../aspose.cells.charts/chartframe/defaultheight/) { get; } | (**Obsolete.**) Represents height of default position in units of 1/4000 of the chart area. |
| [DefaultHeightRatioToChart](../../aspose.cells.charts/chartframe/defaultheightratiotochart/) { get; } | Represents height of default position in units of Fraction of the chart area. |
| [DefaultWidth](../../aspose.cells.charts/chartframe/defaultwidth/) { get; } | (**Obsolete.**) Represents width of default position in units of 1/4000 of the chart area. |
| [DefaultWidthRatioToChart](../../aspose.cells.charts/chartframe/defaultwidthratiotochart/) { get; } | Represents width of default position in units of Fraction of the chart area. |
| [DefaultX](../../aspose.cells.charts/chartframe/defaultx/) { get; } | (**Obsolete.**) Represents x of default position in units of 1/4000 of the chart area. |
| [DefaultXRatioToChart](../../aspose.cells.charts/chartframe/defaultxratiotochart/) { get; } | Represents x of default position in units of Fraction of the chart area. |
| [DefaultY](../../aspose.cells.charts/chartframe/defaulty/) { get; } | (**Obsolete.**) Represents y of default position in units of 1/4000 of the chart area. |
| [DefaultYRatioToChart](../../aspose.cells.charts/chartframe/defaultyratiotochart/) { get; } | Represents y of default position in units of Fraction of the chart area. |
| virtual [Font](../../aspose.cells.charts/chartframe/font/) { get; } | Gets a [`Font`](./font/) object of the specified ChartFrame object. |
| virtual [Height](../../aspose.cells.charts/chartframe/height/) { get; set; } | (**Obsolete.**) Gets or sets the height of frame in units of 1/4000 of the chart area. |
| virtual [HeightPixel](../../aspose.cells.charts/chartframe/heightpixel/) { get; set; } | Gets or sets the height of frame in units of Pixel. |
| virtual [HeightRatioToChart](../../aspose.cells.charts/chartframe/heightratiotochart/) { get; set; } | Gets or sets the height of frame in units of ratio of the chart area. |
| virtual [IsAutomaticSize](../../aspose.cells.charts/chartframe/isautomaticsize/) { get; set; } | Indicates whether the chart frame is automatic sized. |
| [IsDefaultPosBeSet](../../aspose.cells.charts/chartframe/isdefaultposbeset/) { get; } | Indicates whether default position(DefaultX, DefaultY, DefaultWidth and DefaultHeight) are set. |
| [IsInnerMode](../../aspose.cells.charts/chartframe/isinnermode/) { get; set; } | Indicates whether the size of the plot area size includes the tick marks, and the axis labels. False specifies that the size shall determine the size of the plot area, the tick marks, and the axis labels. |
| [Shadow](../../aspose.cells.charts/chartframe/shadow/) { get; set; } | True if the frame has a shadow. |
| [ShapeProperties](../../aspose.cells.charts/chartframe/shapeproperties/) { get; } | Gets the [`ShapeProperties`](./shapeproperties/) object. |
| virtual [TextFont](../../aspose.cells.charts/chartframe/textfont/) { get; } | (**Obsolete.**) Gets a [`Font`](./font/) object of the specified ChartFrame object. |
| virtual [TextOptions](../../aspose.cells.charts/chartframe/textoptions/) { get; } | Gets and sets the options of the text. |
| virtual [Width](../../aspose.cells.charts/chartframe/width/) { get; set; } | (**Obsolete.**) Gets or sets the width of frame in units of 1/4000 of the chart area. |
| virtual [WidthPixel](../../aspose.cells.charts/chartframe/widthpixel/) { get; set; } | Gets or sets the width of frame in units of Pixel. |
| virtual [WidthRatioToChart](../../aspose.cells.charts/chartframe/widthratiotochart/) { get; set; } | Gets or sets the width of frame in units of ratio of the chart area. |
| virtual [X](../../aspose.cells.charts/chartframe/x/) { get; set; } | (**Obsolete.**) Gets or sets the x coordinate of the upper left corner in units of 1/4000 of the chart area. |
| virtual [XPixel](../../aspose.cells.charts/chartframe/xpixel/) { get; set; } | Gets or sets the x coordinate of the upper left corner in units of Pixel. |
| virtual [XRatioToChart](../../aspose.cells.charts/chartframe/xratiotochart/) { get; set; } | Gets or sets the x coordinate of the upper left corner in units of ratio of the chart area. |
| virtual [Y](../../aspose.cells.charts/chartframe/y/) { get; set; } | (**Obsolete.**) Gets or sets the y coordinate of the upper left corner in units of 1/4000 of the chart area. |
| virtual [YPixel](../../aspose.cells.charts/chartframe/ypixel/) { get; set; } | Gets or sets the y coordinate of the upper left corner in units of Pixel. |
| virtual [YRatioToChart](../../aspose.cells.charts/chartframe/yratiotochart/) { get; set; } | Gets or sets the y coordinate of the upper left corner in units of ratio of the chart area. |
## Methods
| Name | Description |
| --- | --- |
| virtual [SetPositionAuto](../../aspose.cells.charts/chartframe/setpositionauto/)() | Set position of the frame to automatic |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;
using System;
using System.Drawing;
public class ChartFrameDemo
{
public static void ChartFrameExample()
{
// Create a new workbook
Workbook workbook = new Workbook();
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
// Access the chart frame
ChartFrame chartFrame = chart.ChartArea;
// Set properties of the chart frame
chartFrame.IsInnerMode = false;
chartFrame.AutoScaleFont = true;
chartFrame.BackgroundMode = BackgroundMode.Transparent;
chartFrame.IsAutomaticSize = true;
chartFrame.X = 1000; // 1/4000 of the chart area
chartFrame.Y = 1000; // 1/4000 of the chart area
chartFrame.Width = 3000; // 1/4000 of the chart area
chartFrame.Height = 2000; // 1/4000 of the chart area
chartFrame.Shadow = true;
// Access and modify the border of the chart frame
Line border = chartFrame.Border;
border.Color = Color.Red;
border.Style = LineType.Solid;
// Access and modify the area of the chart frame
Area area = chartFrame.Area;
area.ForegroundColor = Color.Yellow;
area.BackgroundColor = Color.Blue;
// Access and modify the font of the chart frame
Aspose.Cells.Font font = chartFrame.TextFont;
font.Name = "Arial";
font.Size = 12;
font.IsBold = true;
font.Color = Color.Green;
// Save the workbook
workbook.Save("ChartFrameExample.xlsx");
workbook.Save("ChartFrameExample.pdf");
}
}
}
```
### See Also
* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)
