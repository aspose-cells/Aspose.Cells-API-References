---
title: FillFormat
second_title: Aspose.Cells for .NET API Reference
description: Encapsulates the object that represents fill formatting for a shape.
type: docs
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
| [FillType](../../aspose.cells.drawing/fillformat/filltype) { get; set; } | Gets and sets fill type |
| [GradientColor1](../../aspose.cells.drawing/fillformat/gradientcolor1) { get; } | Returns the gradient color 1 for the specified fill. |
| [GradientColor2](../../aspose.cells.drawing/fillformat/gradientcolor2) { get; } | Returns the gradient color 2 for the specified fill. |
| [GradientColorType](../../aspose.cells.drawing/fillformat/gradientcolortype) { get; } | Returns the gradient color type for the specified fill. |
| [GradientDegree](../../aspose.cells.drawing/fillformat/gradientdegree) { get; } | Returns the gradient degree for the specified fill. Only applies for Excel 2007. |
| [GradientFill](../../aspose.cells.drawing/fillformat/gradientfill) { get; } | Gets [`GradientFill`](./gradientfill) object. |
| [GradientStyle](../../aspose.cells.drawing/fillformat/gradientstyle) { get; } | Returns the gradient style for the specified fill. |
| [GradientVariant](../../aspose.cells.drawing/fillformat/gradientvariant) { get; } | Returns the gradient variant for the specified fill. Only applies for Excel 2007. |
| [ImageData](../../aspose.cells.drawing/fillformat/imagedata) { get; set; } | Gets and sets the picture image data. |
| [Pattern](../../aspose.cells.drawing/fillformat/pattern) { get; set; } | Represents an area's display pattern. |
| [PatternFill](../../aspose.cells.drawing/fillformat/patternfill) { get; } | Gets [`PatternFill`](./patternfill) object. |
| [PictureFormatType](../../aspose.cells.drawing/fillformat/pictureformattype) { get; set; } | Gets and sets the picture format type. |
| [PresetColor](../../aspose.cells.drawing/fillformat/presetcolor) { get; } | Returns the gradient preset color for the specified fill. |
| [Scale](../../aspose.cells.drawing/fillformat/scale) { get; set; } | Gets and sets the picture format scale. |
| [SetType](../../aspose.cells.drawing/fillformat/settype) { get; set; } | (**Obsolete.**) Gets the fill format set type. |
| [SolidFill](../../aspose.cells.drawing/fillformat/solidfill) { get; } | Gets [`SolidFill`](./solidfill) object. |
| [Texture](../../aspose.cells.drawing/fillformat/texture) { get; set; } | Represents the texture type for the specified fill. |
| [TextureFill](../../aspose.cells.drawing/fillformat/texturefill) { get; } | Gets [`TextureFill`](./texturefill) object. |
| [Transparency](../../aspose.cells.drawing/fillformat/transparency) { get; set; } | Returns or sets the degree of transparency of the area as a value from 0.0 (opaque) through 1.0 (clear). |
| [Type](../../aspose.cells.drawing/fillformat/type) { get; set; } | (**Obsolete.**) Gets and sets the fill type. |

## Methods

| Name | Description |
| --- | --- |
| override [Equals](../../aspose.cells.drawing/fillformat/equals)(object) |  |
| override [GetHashCode](../../aspose.cells.drawing/fillformat/gethashcode)() | Gets the hash code. |
| [SetOneColorGradient](../../aspose.cells.drawing/fillformat/setonecolorgradient)(Color, double, GradientStyleType, int) | Sets the specified fill to a one-color gradient. Only applies for Excel 2007. |
| [SetPresetColorGradient](../../aspose.cells.drawing/fillformat/setpresetcolorgradient)(GradientPresetType, GradientStyleType, int) | Sets the specified fill to a preset-color gradient. Only applies for Excel 2007. |
| [SetTwoColorGradient](../../aspose.cells.drawing/fillformat/settwocolorgradient#settwocolorgradient_1)(Color, Color, GradientStyleType, int) | Sets the specified fill to a two-color gradient. Only applies for Excel 2007. |
| [SetTwoColorGradient](../../aspose.cells.drawing/fillformat/settwocolorgradient#settwocolorgradient)(Color, double, Color, double, GradientStyleType, int) | Sets the specified fill to a two-color gradient. Only applies for Excel 2007. |

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
