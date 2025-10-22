##Class FillFormat
Aspose.Cells.Drawing.FillFormat class. Encapsulates the object that represents fill formatting for a shape
## FillFormat class
Encapsulates the object that represents fill formatting for a shape.
```csharp
public class FillFormat
```
## Properties
| Name | Description |
| --- | --- |
| [FillType](../../aspose.cells.drawing/fillformat/filltype/) { get; set; } | Gets and sets fill type |
| [GradientColor1](../../aspose.cells.drawing/fillformat/gradientcolor1/) { get; } | Returns the gradient color 1 for the specified fill. |
| [GradientColor2](../../aspose.cells.drawing/fillformat/gradientcolor2/) { get; } | Returns the gradient color 2 for the specified fill. |
| [GradientColorType](../../aspose.cells.drawing/fillformat/gradientcolortype/) { get; } | Returns the gradient color type for the specified fill. |
| [GradientDegree](../../aspose.cells.drawing/fillformat/gradientdegree/) { get; } | Returns the gradient degree for the specified fill. Only applies for Excel 2007. |
| [GradientFill](../../aspose.cells.drawing/fillformat/gradientfill/) { get; } | Gets [`GradientFill`](./gradientfill/) object. |
| [GradientStyle](../../aspose.cells.drawing/fillformat/gradientstyle/) { get; } | Returns the gradient style for the specified fill. |
| [GradientVariant](../../aspose.cells.drawing/fillformat/gradientvariant/) { get; } | Returns the gradient variant for the specified fill. Only applies for Excel 2007. |
| [ImageData](../../aspose.cells.drawing/fillformat/imagedata/) { get; set; } | Gets and sets the picture image data. |
| [Pattern](../../aspose.cells.drawing/fillformat/pattern/) { get; set; } | Represents an area's display pattern. |
| [PatternFill](../../aspose.cells.drawing/fillformat/patternfill/) { get; } | Gets [`PatternFill`](./patternfill/) object. |
| [PictureFormatType](../../aspose.cells.drawing/fillformat/pictureformattype/) { get; set; } | Gets and sets the picture format type. |
| [PresetColor](../../aspose.cells.drawing/fillformat/presetcolor/) { get; } | Returns the gradient preset color for the specified fill. |
| [Scale](../../aspose.cells.drawing/fillformat/scale/) { get; set; } | Gets and sets the picture format scale. |
| [SetType](../../aspose.cells.drawing/fillformat/settype/) { get; set; } | (**Obsolete.**) Gets the fill format set type. |
| [SolidFill](../../aspose.cells.drawing/fillformat/solidfill/) { get; } | Gets [`SolidFill`](./solidfill/) object. |
| [Texture](../../aspose.cells.drawing/fillformat/texture/) { get; set; } | Represents the texture type for the specified fill. |
| [TextureFill](../../aspose.cells.drawing/fillformat/texturefill/) { get; } | Gets [`TextureFill`](./texturefill/) object. |
| [Transparency](../../aspose.cells.drawing/fillformat/transparency/) { get; set; } | Returns or sets the degree of transparency of the area as a value from 0.0 (opaque) through 1.0 (clear). |
| [Type](../../aspose.cells.drawing/fillformat/type/) { get; set; } | (**Obsolete.**) Gets and sets the fill type. |
## Methods
| Name | Description |
| --- | --- |
| override [Equals](../../aspose.cells.drawing/fillformat/equals/)(object) |  |
| override [GetHashCode](../../aspose.cells.drawing/fillformat/gethashcode/)() | Gets the hash code. |
| [SetOneColorGradient](../../aspose.cells.drawing/fillformat/setonecolorgradient/)(Color, double, GradientStyleType, int) | Sets the specified fill to a one-color gradient. Only applies for Excel 2007. |
| [SetPresetColorGradient](../../aspose.cells.drawing/fillformat/setpresetcolorgradient/)(GradientPresetType, GradientStyleType, int) | Sets the specified fill to a preset-color gradient. Only applies for Excel 2007. |
| [SetTwoColorGradient](../../aspose.cells.drawing/fillformat/settwocolorgradient/#settwocolorgradient_1)(Color, Color, GradientStyleType, int) | Sets the specified fill to a two-color gradient. Only applies for Excel 2007. |
| [SetTwoColorGradient](../../aspose.cells.drawing/fillformat/settwocolorgradient/#settwocolorgradient)(Color, double, Color, double, GradientStyleType, int) | Sets the specified fill to a two-color gradient. Only applies for Excel 2007. |
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
using System.Drawing;
namespace AsposeCellsExamples
{
public class DrawingClassFillFormatDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data to cells
worksheet.Cells["A1"].PutValue(50);
worksheet.Cells["A2"].PutValue(100);
worksheet.Cells["A3"].PutValue(150);
worksheet.Cells["A4"].PutValue(200);
worksheet.Cells["B1"].PutValue(60);
worksheet.Cells["B2"].PutValue(32);
worksheet.Cells["B3"].PutValue(50);
worksheet.Cells["B4"].PutValue(40);
worksheet.Cells["C1"].PutValue("Q1");
worksheet.Cells["C2"].PutValue("Q2");
worksheet.Cells["C3"].PutValue("Y1");
worksheet.Cells["C4"].PutValue("Y2");
// Add a column chart to the worksheet
int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
// Add data series to the chart
int seriesIndex = chart.NSeries.Add("A1:B4", true);
chart.NSeries.CategoryData = "C1:C4";
// Apply gradient fill to the series area
chart.NSeries[seriesIndex].Area.FillFormat.SetOneColorGradient(System.Drawing.Color.Lime, 1,
GradientStyleType.Horizontal, 1);
// Save the workbook
workbook.Save("FillFormatDemo.xlsx");
}
}
}
```
### See Also
* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)
