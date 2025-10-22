##ThreeDFormat.ContourColor
ThreeDFormat property. Gets and sets the contour color on a shape
## ThreeDFormat.ContourColor property
Gets and sets the contour color on a shape.
```csharp
public CellsColor ContourColor { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System;
public class ThreeDFormatPropertyContourColorDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a shape to demonstrate 3D formatting
Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.TextBox, 1, 1, 200, 100, 0, 0);
shape.Text = "3D ContourColor Demo";
// Get the ThreeDFormat of the shape
ThreeDFormat threeDFormat = shape.ThreeDFormat;
// Configure basic 3D properties
threeDFormat.TopBevelType = BevelType.ArtDeco;
threeDFormat.TopBevelWidth = 10;
threeDFormat.TopBevelHeight = 10;
threeDFormat.ContourWidth = 2;
try
{
// Get current ContourColor value
CellsColor contourColor = threeDFormat.ContourColor;
Console.WriteLine($"Initial ContourColor - Type: {contourColor.Type}, ARGB: {contourColor.Argb}");
// Create new color by modifying existing one
contourColor.Argb = System.Drawing.Color.Red.ToArgb();
contourColor.Transparency = 0.5;
threeDFormat.ContourColor = contourColor;
// Display the new ContourColor value
Console.WriteLine($"New ContourColor - Type: {threeDFormat.ContourColor.Type}, ARGB: {threeDFormat.ContourColor.Argb}");
// Save the workbook to see the effects
workbook.Save("ThreeDFormatContourColorDemo.xlsx");
}
catch (Exception ex)
{
Console.WriteLine($"Error: {ex.Message}");
}
}
}
}
```
### See Also
* class [CellsColor](../../../aspose.cells/cellscolor/)
* class [ThreeDFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
