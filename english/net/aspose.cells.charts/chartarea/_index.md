---
title: ChartArea
second_title: Aspose.Cells for .NET API Reference
description: Encapsulates the object that represents the chart area in the worksheet.
type: docs
weight: 440
url: /net/aspose.cells.charts/chartarea/
---
## ChartArea class

Encapsulates the object that represents the chart area in the worksheet.

```csharp
public class ChartArea : ChartFrame
```

## Properties

| Name | Description |
| --- | --- |
| virtual [Area](../../aspose.cells.charts/chartframe/area) { get; } | Gets the [`area`](../chartframe/area).(Inherited from [`ChartFrame`](../chartframe).) |
| virtual [AutoScaleFont](../../aspose.cells.charts/chartframe/autoscalefont) { get; set; } | True if the text in the object changes font size when the object size changes. The default value is True.(Inherited from [`ChartFrame`](../chartframe).) |
| [Background](../../aspose.cells.charts/chartframe/background) { get; set; } | (**Obsolete.**) Gets and sets the display mode of the background(Inherited from [`ChartFrame`](../chartframe).) |
| [BackgroundMode](../../aspose.cells.charts/chartframe/backgroundmode) { get; set; } | Gets and sets the display mode of the background(Inherited from [`ChartFrame`](../chartframe).) |
| virtual [Border](../../aspose.cells.charts/chartframe/border) { get; } | Gets the [`border`](../../aspose.cells.drawing/line).(Inherited from [`ChartFrame`](../chartframe).) |
| [DefaultHeight](../../aspose.cells.charts/chartframe/defaultheight) { get; } | Represents height of default position(Inherited from [`ChartFrame`](../chartframe).) |
| [DefaultWidth](../../aspose.cells.charts/chartframe/defaultwidth) { get; } | Represents width of default position(Inherited from [`ChartFrame`](../chartframe).) |
| [DefaultX](../../aspose.cells.charts/chartframe/defaultx) { get; } | Represents x of default position(Inherited from [`ChartFrame`](../chartframe).) |
| [DefaultY](../../aspose.cells.charts/chartframe/defaulty) { get; } | Represents y of default position(Inherited from [`ChartFrame`](../chartframe).) |
| override [Font](../../aspose.cells.charts/chartarea/font) { get; } | Gets a [`Font`](./font) object of the specified chartarea object. |
| override [Height](../../aspose.cells.charts/chartarea/height) { get; set; } | Gets or sets the vertical offset from its lower right corner row. |
| virtual [IsAutomaticSize](../../aspose.cells.charts/chartframe/isautomaticsize) { get; set; } | Indicates whether the chart frame is automatic sized.(Inherited from [`ChartFrame`](../chartframe).) |
| [IsDefaultPosBeSet](../../aspose.cells.charts/chartframe/isdefaultposbeset) { get; } | Indicates whether default position(DefaultX, DefaultY, DefaultWidth and DefaultHeight) are set.(Inherited from [`ChartFrame`](../chartframe).) |
| [IsInnerMode](../../aspose.cells.charts/chartframe/isinnermode) { get; set; } | Indicates whether the size of the plot area size includes the tick marks, and the axis labels. False specifies that the size shall determine the size of the plot area, the tick marks, and the axis labels.(Inherited from [`ChartFrame`](../chartframe).) |
| [Shadow](../../aspose.cells.charts/chartframe/shadow) { get; set; } | True if the frame has a shadow.(Inherited from [`ChartFrame`](../chartframe).) |
| [ShapeProperties](../../aspose.cells.charts/chartframe/shapeproperties) { get; } | Gets the [`ShapeProperties`](../chartframe/shapeproperties) object.(Inherited from [`ChartFrame`](../chartframe).) |
| virtual [TextFont](../../aspose.cells.charts/chartframe/textfont) { get; } | (**Obsolete.**) Gets a [`Font`](../chartframe/font) object of the specified ChartFrame object.(Inherited from [`ChartFrame`](../chartframe).) |
| virtual [TextOptions](../../aspose.cells.charts/chartframe/textoptions) { get; } | Gets and sets the options of the text.(Inherited from [`ChartFrame`](../chartframe).) |
| override [Width](../../aspose.cells.charts/chartarea/width) { get; set; } | Gets or sets the horizontal offset from its lower right corner column. |
| override [X](../../aspose.cells.charts/chartarea/x) { get; set; } | Gets or gets the horizontal offset from its upper left corner column. |
| override [Y](../../aspose.cells.charts/chartarea/y) { get; set; } | Gets or gets the vertical offset from its upper left corner row. |

## Methods

| Name | Description |
| --- | --- |
| virtual [SetPositionAuto](../../aspose.cells.charts/chartframe/setpositionauto)() | Set position of the frame to automatic(Inherited from [`ChartFrame`](../chartframe).) |

### Examples

```csharp

[C#]

//Instantiating a Workbook object
Workbook workbook = new Workbook();

//Obtaining the reference of the first worksheet
Worksheet worksheet = workbook.Worksheets[0];

//Adding a sample value to "A1" cell
worksheet.Cells["A1"].PutValue(50);

//Adding a sample value to "A2" cell
worksheet.Cells["A2"].PutValue(100);

//Adding a sample value to "A3" cell
worksheet.Cells["A3"].PutValue(150);

//Adding a sample value to "B1" cell
worksheet.Cells["B1"].PutValue(60);

//Adding a sample value to "B2" cell
worksheet.Cells["B2"].PutValue(32);

//Adding a sample value to "B3" cell
worksheet.Cells["B3"].PutValue(50);

//Adding a chart to the worksheet
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);

//Accessing the instance of the newly added chart
Chart chart = worksheet.Charts[chartIndex];

//Adding NSeries (chart data source) to the chart ranging from "A1" cell to "B3"
chart.NSeries.Add("A1:B3", true);

//Getting Chart Area
ChartArea chartArea = chart.ChartArea;

//Setting the foreground color of the chart area
chartArea.Area.ForegroundColor = Color.Yellow;

//Setting Chart Area Shadow
chartArea.Shadow = true;

//Saving the Excel file
workbook.Save("book1.xls");

[VB.NET]

'Instantiating a Workbook object
Dim workbook As Workbook = New Workbook()

'Obtaining the reference of the first worksheet
Dim worksheet As Worksheet = workbook.Worksheets(0)

'Adding a sample value to "A1" cell
worksheet.Cells("A1").PutValue(50)

'Adding a sample value to "A2" cell
worksheet.Cells("A2").PutValue(100)

'Adding a sample value to "A3" cell
worksheet.Cells("A3").PutValue(150)

'Adding a sample value to "B1" cell
worksheet.Cells("B1").PutValue(60)

'Adding a sample value to "B2" cell
worksheet.Cells("B2").PutValue(32)

'Adding a sample value to "B3" cell
worksheet.Cells("B3").PutValue(50)

'Adding a chart to the worksheet
Dim chartIndex As Integer = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5)

'Accessing the instance of the newly added chart
Dim chart As Chart = worksheet.Charts(chartIndex)

'Adding NSeries (chart data source) to the chart ranging from "A1" cell to "B3"
chart.NSeries.Add("A1:B3", True)

'Getting Chart Area
Dim chartArea As ChartArea = chart.ChartArea

'Setting the foreground color of the chart area
chartArea.Area.ForegroundColor = Color.Yellow

'Setting Chart Area Shadow
chartArea.Shadow = True

'Saving the Excel file
workbook.Save("book1.xls")
```

### See Also

* class [ChartFrame](../chartframe)
* namespace [Aspose.Cells.Charts](../../aspose.cells.charts)
* assembly [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
