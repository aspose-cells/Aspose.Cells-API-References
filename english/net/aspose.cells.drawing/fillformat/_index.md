---
title: FillFormat
second_title: Aspose.Cells for .NET API Reference
description: 
type: docs
weight: 1940
url: /net/aspose.cells.drawing/fillformat/
---
## FillFormat class

Encapsulates the object that represents fill formatting for a shape.

```csharp
public class FillFormat
```

## Properties

| Name | Description |
| --- | --- |
| [FillType](filltype) { get; set; } | Gets and sets fill type |
| [GradientColor1](gradientcolor1) { get; } | Returns the gradient color 1 for the specified fill. |
| [GradientColor2](gradientcolor2) { get; } | Returns the gradient color 2 for the specified fill. |
| [GradientColorType](gradientcolortype) { get; } | Returns the gradient color type for the specified fill. |
| [GradientDegree](gradientdegree) { get; } | Returns the gradient degree for the specified fill. Only applies for Excel 2007. |
| [GradientFill](gradientfill) { get; } | Gets [`GradientFill`](./gradientfill) object. |
| [GradientStyle](gradientstyle) { get; } | Returns the gradient style for the specified fill. |
| [GradientVariant](gradientvariant) { get; } | Returns the gradient variant for the specified fill. Only applies for Excel 2007. |
| [ImageData](imagedata) { get; set; } | Gets and sets the picture image data. |
| [Pattern](pattern) { get; set; } | Represents an area's display pattern. |
| [PatternFill](patternfill) { get; } | Gets [`PatternFill`](./patternfill) object. |
| [PictureFormatType](pictureformattype) { get; set; } | Gets and sets the picture format type. |
| [PresetColor](presetcolor) { get; } | Returns the gradient preset color for the specified fill. |
| [Scale](scale) { get; set; } | Gets and sets the picture format scale. |
| [SolidFill](solidfill) { get; } | Gets [`SolidFill`](./solidfill) object. |
| [Texture](texture) { get; set; } | Represents the texture type for the specified fill. |
| [TextureFill](texturefill) { get; } | Gets [`TextureFill`](./texturefill) object. |
| [Transparency](transparency) { get; set; } | Returns or sets the degree of transparency of the area as a value from 0.0 (opaque) through 1.0 (clear). |

## Methods

| Name | Description |
| --- | --- |
| override [Equals](equals)(object) |  |
| override [GetHashCode](gethashcode)() | Gets the hash code. |
| [SetOneColorGradient](setonecolorgradient)(Color, double, GradientStyleType, int) | Sets the specified fill to a one-color gradient. Only applies for Excel 2007. |
| [SetPresetColorGradient](setpresetcolorgradient)(GradientPresetType, GradientStyleType, int) | Sets the specified fill to a preset-color gradient. Only applies for Excel 2007. |
| [SetTwoColorGradient](settwocolorgradient)(Color, Color, GradientStyleType, int) | Sets the specified fill to a two-color gradient. Only applies for Excel 2007. |
| [SetTwoColorGradient](settwocolorgradient)(Color, double, Color, double, GradientStyleType, int) | Sets the specified fill to a two-color gradient. Only applies for Excel 2007. |

### Examples

```csharp

[C#]

//Instantiating a Workbook object
Workbook workbook = new Workbook();
//Adding a new worksheet to the Excel object
int sheetIndex = workbook.Worksheets.Add();
//Obtaining the reference of the newly added worksheet by passing its sheet index
Worksheet worksheet = workbook.Worksheets[sheetIndex];
//Adding a sample value to "A1" cell
worksheet.Cells["A1"].PutValue(50);
//Adding a sample value to "A2" cell
worksheet.Cells["A2"].PutValue(100);
//Adding a sample value to "A3" cell
worksheet.Cells["A3"].PutValue(150);
//Adding a sample value to "A4" cell
worksheet.Cells["A4"].PutValue(200);
//Adding a sample value to "B1" cell
worksheet.Cells["B1"].PutValue(60);
//Adding a sample value to "B2" cell
worksheet.Cells["B2"].PutValue(32);
//Adding a sample value to "B3" cell
worksheet.Cells["B3"].PutValue(50);
//Adding a sample value to "B4" cell
worksheet.Cells["B4"].PutValue(40);
//Adding a sample value to "C1" cell as category data
worksheet.Cells["C1"].PutValue("Q1");
//Adding a sample value to "C2" cell as category data
worksheet.Cells["C2"].PutValue("Q2");
//Adding a sample value to "C3" cell as category data
worksheet.Cells["C3"].PutValue("Y1");
//Adding a sample value to "C4" cell as category data
worksheet.Cells["C4"].PutValue("Y2");
//Adding a chart to the worksheet
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
//Accessing the instance of the newly added chart
Chart chart = worksheet.Charts[chartIndex];
//Adding NSeries (chart data source) to the chart ranging from "A1" cell to "B4"
int seriesIndex = chart.NSeries.Add("A1:B4", true);
//Setting the data source for the category data of NSeries
chart.NSeries.CategoryData = "C1:C4";
//Filling the area of the 2nd NSeries with a gradient
chart.NSeries[seriesIndex].Area.FillFormat.SetOneColorGradient(Color.Lime, 1, GradientStyleType.Horizontal, 1);

[Visual Basic]

Instantiating a Workbook object
Dim workbook As Workbook = New Workbook()
'Adding a new worksheet to the Excel object
Dim sheetIndex As Int32 = workbook.Worksheets.Add()
'Obtaining the reference of the newly added worksheet by passing its sheet index
Dim worksheet As Worksheet = workbook.Worksheets(sheetIndex)
'Adding a sample value to "A1" cell
worksheet.Cells("A1").PutValue(50)
'Adding a sample value to "A2" cell
worksheet.Cells("A2").PutValue(100)
'Adding a sample value to "A3" cell
worksheet.Cells("A3").PutValue(150)
'Adding a sample value to "A4" cell
worksheet.Cells("A4").PutValue(200)
'Adding a sample value to "B1" cell
worksheet.Cells("B1").PutValue(60)
'Adding a sample value to "B2" cell
worksheet.Cells("B2").PutValue(32)
'Adding a sample value to "B3" cell
worksheet.Cells("B3").PutValue(50)
'Adding a sample value to "B4" cell
worksheet.Cells("B4").PutValue(40)
'Adding a sample value to "C1" cell as category data
worksheet.Cells("C1").PutValue("Q1")
'Adding a sample value to "C2" cell as category data
worksheet.Cells("C2").PutValue("Q2")
'Adding a sample value to "C3" cell as category data
worksheet.Cells("C3").PutValue("Y1")
'Adding a sample value to "C4" cell as category data
worksheet.Cells("C4").PutValue("Y2")
'Adding a chart to the worksheet
Dim chartIndex As Int32 = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5)
'Accessing the instance of the newly added chart
Dim chart As Chart = worksheet.Charts(chartIndex)
'Adding NSeries (chart data source) to the chart ranging from "A1" cell to "B4"
Dim seriesIndex As Int32 = chart.NSeries.Add("A1:B4", True)
'Setting the data source for the category data of NSeries
chart.NSeries.CategoryData = "C1:C4"
'Filling the area of the 2nd NSeries with a gradient
chart.NSeries(seriesIndex).Area.FillFormat.SetOneColorGradient(Color.Lime, 1, GradientStyleType.Horizontal, 1)
```

### See Also

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing)
* assembly [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
