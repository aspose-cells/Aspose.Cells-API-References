##Class MsoFillFormat
Aspose.Cells.Drawing.MsoFillFormat class. Represents fill formatting for a shape
## MsoFillFormat class
Represents fill formatting for a shape.
```csharp
public class MsoFillFormat
```
## Properties
| Name | Description |
| --- | --- |
| [BackColor](../../aspose.cells.drawing/msofillformat/backcolor/) { get; set; } | Gets and sets the file back color. |
| [ForeColor](../../aspose.cells.drawing/msofillformat/forecolor/) { get; set; } | Gets and sets the fill fore color. |
| [ImageData](../../aspose.cells.drawing/msofillformat/imagedata/) { get; set; } | Gets and sets the Texture and Picture fill data. |
| [IsVisible](../../aspose.cells.drawing/msofillformat/isvisible/) { get; set; } | Indicates whether there is fill. |
| [Texture](../../aspose.cells.drawing/msofillformat/texture/) { get; } | Gets the texture fill type. |
| [Transparency](../../aspose.cells.drawing/msofillformat/transparency/) { get; set; } | Returns or sets the degree of transparency of the specified fill as a value from 0.0 (opaque) through 1.0 (clear). |
## Methods
| Name | Description |
| --- | --- |
| [SetOneColorGradient](../../aspose.cells.drawing/msofillformat/setonecolorgradient/)(Color, double, GradientStyleType, int) | Sets the specified fill to a one-color gradient. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System;
using System.Drawing;
public class MsoFillFormatDemo
{
public static void MsoFillFormatExample()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add an arc shape to the worksheet
Aspose.Cells.Drawing.ArcShape arcShape = worksheet.Shapes.AddArc(2, 0, 2, 0, 130, 130);
// Access the fill format of the shape
MsoFillFormat fillFormat = arcShape.FillFormat;
// Set the fill fore color
fillFormat.ForeColor = Color.Blue;
// Set the fill back color
fillFormat.BackColor = Color.LightBlue;
// Set the transparency
fillFormat.Transparency = 0.5;
// Check if the fill is visible
bool isVisible = fillFormat.IsVisible;
Console.WriteLine("Is Fill Visible: " + isVisible);
// Set a one-color gradient fill
fillFormat.SetOneColorGradient(Color.Green, 0.3, GradientStyleType.Horizontal, 1);
// Save the workbook
workbook.Save("MsoFillFormatExample.xlsx");
}
}
}
```
### See Also
* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)
