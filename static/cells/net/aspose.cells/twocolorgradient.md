##Class TwoColorGradient
Aspose.Cells.TwoColorGradient class. Represents two color gradient
## TwoColorGradient class
Represents two color gradient.
```csharp
public class TwoColorGradient
```
## Constructors
| Name | Description |
| --- | --- |
| [TwoColorGradient](twocolorgradient/)(Color, Color, GradientStyleType, int) |  |
## Properties
| Name | Description |
| --- | --- |
| [Color1](../../aspose.cells/twocolorgradient/color1/) { get; set; } | Gets and sets the first gradient color. |
| [Color2](../../aspose.cells/twocolorgradient/color2/) { get; set; } | Gets and sets the second gradient color. |
| [GradientStyleType](../../aspose.cells/twocolorgradient/gradientstyletype/) { get; set; } | Gets and sets gradient shading style. |
| [Variant](../../aspose.cells/twocolorgradient/variant/) { get; set; } | Gets and sets the gradient variant. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System;
using System.Drawing;
public class CellsClassTwoColorGradientDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Initialize TwoColorGradient with constructor parameters
TwoColorGradient gradient = new TwoColorGradient(
Color.LightSkyBlue,
Color.DarkBlue,
GradientStyleType.DiagonalUp,
2);
// Modify gradient properties after initialization
gradient.GradientStyleType = GradientStyleType.DiagonalDown;
// Create cell style and apply gradient
Style style = workbook.CreateStyle();
style.SetTwoColorGradient(gradient.Color1, gradient.Color2, gradient.GradientStyleType, gradient.Variant);
// Apply style to cell and add content
Cell cell = worksheet.Cells["B2"];
cell.PutValue("Aspose.Cells TwoColorGradient Demo");
cell.SetStyle(style);
// Adjust cell dimensions for visibility
worksheet.Cells.SetRowHeight(1, 45);
worksheet.Cells.SetColumnWidth(1, 55);
// Save result with gradient formatting
workbook.Save("TwoColorGradientDemo.xlsx");
}
}
}
```
### See Also
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
