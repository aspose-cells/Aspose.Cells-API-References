##CellsColor.SetTintOfShapeColor
CellsColor method. Set the tint of the shape color
## CellsColor.SetTintOfShapeColor method
Set the tint of the shape color
```csharp
public void SetTintOfShapeColor(double tint)
```
| Parameter | Type | Description |
| --- | --- | --- |
| tint | Double |  |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System;
public class CellsColorMethodSetTintOfShapeColorWithDoubleDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a shape to the worksheet
Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 100);
try
{
// Get the shape's fill color
CellsColor shapeColor = shape.Fill.SolidFill.CellsColor;
// Set the color to be treated as shape color
shapeColor.IsShapeColor = true;
// Set the tint of the shape color (valid range is -1.0 to 1.0)
shapeColor.SetTintOfShapeColor(0.5); // Lighten the color by 50%
Console.WriteLine("SetTintOfShapeColor method executed successfully with parameter 0.5");
// Display the effect by changing the shape's fill color
shape.Fill.SolidFill.Color = System.Drawing.Color.Blue;
}
catch (Exception ex)
{
Console.WriteLine($"Error executing SetTintOfShapeColor method: {ex.Message}");
}
// Save the result
workbook.Save("SetTintOfShapeColorWithDoubleDemo.xlsx");
}
}
}
```
### See Also
* class [CellsColor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
