---
title: Class Line
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.Drawing.Line class. Encapsulates the object that represents the line format
type: docs
url: /net/aspose.cells.drawing/line/
---
## Line class

Encapsulates the object that represents the line format.

```csharp
public class Line
```

## Properties

| Name | Description |
| --- | --- |
| [BeginArrowLength](../../aspose.cells.drawing/line/beginarrowlength/) { get; set; } | Specifies the length of the arrowhead for the begin of a line. |
| [BeginArrowWidth](../../aspose.cells.drawing/line/beginarrowwidth/) { get; set; } | Specifies the width of the arrowhead for the begin of a line. |
| [BeginType](../../aspose.cells.drawing/line/begintype/) { get; set; } | Specifies an arrowhead for the begin of a line. |
| [CapType](../../aspose.cells.drawing/line/captype/) { get; set; } | Specifies the ending caps. |
| [Color](../../aspose.cells.drawing/line/color/) { get; set; } | Represents the Color of the line. |
| [CompoundType](../../aspose.cells.drawing/line/compoundtype/) { get; set; } | Specifies the compound line type |
| [DashType](../../aspose.cells.drawing/line/dashtype/) { get; set; } | Specifies the dash line type |
| [EndArrowLength](../../aspose.cells.drawing/line/endarrowlength/) { get; set; } | Specifies the length of the arrowhead for the end of a line. |
| [EndArrowWidth](../../aspose.cells.drawing/line/endarrowwidth/) { get; set; } | Specifies the width of the arrowhead for the end of a line. |
| [EndType](../../aspose.cells.drawing/line/endtype/) { get; set; } | Specifies an arrowhead for the end of a line. |
| [FormattingType](../../aspose.cells.drawing/line/formattingtype/) { get; set; } | Gets or sets format type. |
| [GradientFill](../../aspose.cells.drawing/line/gradientfill/) { get; } | Represents gradient fill. |
| [IsAuto](../../aspose.cells.drawing/line/isauto/) { get; set; } | Indicates whether this line style is auto assigned. |
| [IsAutomaticColor](../../aspose.cells.drawing/line/isautomaticcolor/) { get; } | Indicates whether the color of line is automatic assigned. |
| [IsVisible](../../aspose.cells.drawing/line/isvisible/) { get; set; } | Represents whether the line is visible. |
| [JoinType](../../aspose.cells.drawing/line/jointype/) { get; set; } | Specifies the joining caps. |
| [Style](../../aspose.cells.drawing/line/style/) { get; set; } | Represents the style of the line. |
| [ThemeColor](../../aspose.cells.drawing/line/themecolor/) { get; set; } | Gets and sets the theme color. |
| [Transparency](../../aspose.cells.drawing/line/transparency/) { get; set; } | Returns or sets the degree of transparency of the line as a value from 0.0 (opaque) through 1.0 (clear). |
| [Weight](../../aspose.cells.drawing/line/weight/) { get; set; } | Gets or sets the [`WeightType`](../weighttype/) of the line. |
| [WeightPt](../../aspose.cells.drawing/line/weightpt/) { get; set; } | Gets or sets the weight of the line in unit of points. |
| [WeightPx](../../aspose.cells.drawing/line/weightpx/) { get; set; } | Gets or sets the weight of the line in unit of pixels. |

### Examples

```csharp

[C#]

Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];

Cells cells = sheet.Cells;
cells[0,1].PutValue("Income");
cells[1,0].PutValue("Company A");
cells[2,0].PutValue("Company B");
cells[3,0].PutValue("Company C");
cells[1,1].PutValue(10000);
cells[2,1].PutValue(20000);
cells[3,1].PutValue(30000);

int chartIndex = sheet.Charts.Add(ChartType.Line, 9, 9, 21, 15);
Chart chart = sheet.Charts[chartIndex];
//Add series
chart.NSeries.Add("A2:B4", true);
//Set category data
chart.NSeries.CategoryData = "=Sheet1!$A$2:$A$4";
//Applying a dotted line style on the lines of an NSeries
chart.NSeries[0].Border.Style = LineType.Dot;
chart.NSeries[0].Border.Color = Color.Red;
//Applying a triangular marker style on the data markers of an NSeries
chart.NSeries[0].Marker.MarkerStyle = ChartMarkerType.Triangle;
//Setting the weight of all lines in an NSeries to medium
chart.NSeries[0].Border.Weight = WeightType.MediumLine;

[Visual Basic]

Dim workbook as Workbook = new Workbook()
Dim sheet as Worksheet = workbook.Worksheets(0)

Dim cells as Cells = sheet.Cells
cells(0,1).PutValue("Income")
cells(1,0).PutValue("Company A")
cells(2,0).PutValue("Company B")
cells(3,0).PutValue("Company C")
cells(1,1).PutValue(10000)
cells(2,1).PutValue(20000)
cells(3,1).PutValue(30000)
		
Dim chartIndex as Integer = sheet.Charts.Add(ChartType.Column, 9, 9, 21, 15)    ///
Dim chart as Chart = sheet.Charts(chartIndex)
'Adding NSeries (chart data source) to the chart ranging from "A2" cell to "B4"
chart.NSeries.Add("A2:B4", True)
'Setting the data source for the category data of NSeries
Chart.NSeries.CategoryData = "A2:A4"
'Applying a dotted line style on the lines of an NSeries
chart.NSeries(0).Border.Style = LineType.Dot
chart.NSeries(0).Border.Color = Color.Red
'Applying a triangular marker style on the data markers of an NSeries
chart.NSeries(0).Marker.MarkerStyle = ChartMarkerType.Triangle
'Setting the weight of all lines in an NSeries to medium
chart.NSeries(0).Border.Weight = WeightType.MediumLine
```

### See Also

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


