---
title: Class Area
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.Drawing.Area class. Encapsulates the object that represents an area format
type: docs
url: /net/aspose.cells.drawing/area/
---
## Area class

Encapsulates the object that represents an area format.

```csharp
public class Area
```

## Properties

| Name | Description |
| --- | --- |
| [BackgroundColor](../../aspose.cells.drawing/area/backgroundcolor/) { get; set; } | Gets or sets the background Color of the `Area`. |
| [FillFormat](../../aspose.cells.drawing/area/fillformat/) { get; } | Represents a  object that contains fill formatting properties for the specified chart or shape. |
| [ForegroundColor](../../aspose.cells.drawing/area/foregroundcolor/) { get; set; } | Gets or sets the foreground Color. |
| [Formatting](../../aspose.cells.drawing/area/formatting/) { get; set; } | Represents the formatting of the area. |
| [InvertIfNegative](../../aspose.cells.drawing/area/invertifnegative/) { get; set; } | If the property is true and the value of chart point is a negative number, the foreground color and background color will be exchanged. |
| [Transparency](../../aspose.cells.drawing/area/transparency/) { get; set; } | Returns or sets the degree of transparency of the area as a value from 0.0 (opaque) through 1.0 (clear). |

### Examples

```csharp

[C#]
//Instantiating a Workbook object
Workbook workbook = new Workbook();
//Adding a new worksheet to the Workbook object
int sheetIndex = workbook.Worksheets.Add();
//Obtaining the reference of the newly added worksheet by passing its sheet index
Worksheet worksheet = workbook.Worksheets[sheetIndex];
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
//Setting the foreground color of the plot area
chart.PlotArea.Area.ForegroundColor = Color.Blue;
//Setting the foreground color of the chart area
chart.ChartArea.Area.ForegroundColor = Color.Yellow;
//Setting the foreground color of the 1st NSeries area
chart.NSeries[0].Area.ForegroundColor = Color.Red;
//Setting the foreground color of the area of the 1st NSeries point
chart.NSeries[0].Points[0].Area.ForegroundColor = Color.Cyan;
//Saving the Excel file
workbook.Save("book1.xls");

[Visual Basic]

'Instantiating a Workbook object
Dim workbook As Workbook = New Workbook()
'Adding a new worksheet to the Workbook object
Dim sheetIndex As Integer = workbook.Worksheets.Add()
'Obtaining the reference of the newly added worksheet by passing its sheet index
Dim worksheet As Worksheet = workbook.Worksheets(sheetIndex)
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
'Setting the foreground color of the plot area
chart.PlotArea.Area.ForegroundColor = Color.Blue
'Setting the foreground color of the chart area
chart.ChartArea.Area.ForegroundColor = Color.Yellow
'Setting the foreground color of the 1st NSeries area
chart.NSeries(0).Area.ForegroundColor = Color.Red
'Setting the foreground color of the area of the 1st NSeries point
chart.NSeries(0).Points(0).Area.ForegroundColor = Color.Cyan
'Saving the Excel file
workbook.Save("book1.xls")
```

### See Also

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


