##ShapePath.MoveTo
ShapePath method. Starts a new figure from the specified point without closing the current figure. All subsequent points added to the path are added to this new figure.Unit Pixel
## ShapePath.MoveTo method
Starts a new figure from the specified point without closing the current figure. All subsequent points added to the path are added to this new figure.Unit: Pixel.
```csharp
public void MoveTo(float x, float y)
```
| Parameter | Type | Description |
| --- | --- | --- |
| x | Single | The x-coordinate of the starting point of the figure(Unit: Pixel). |
| y | Single | The y-coordinate of the starting point of the figure(Unit: Pixel). |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System;
public class ShapePathMethodMoveToWithSingleSingleDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
try
{
//Create a new shape path
ShapePath shapePath = new ShapePath();
// Move to starting point
shapePath.MoveTo(10, 10);
// Call LineTo method with (Single, Single) parameters
shapePath.LineTo(50.5f, 10.5f);
shapePath.LineTo(50.5f, 50.5f);
shapePath.LineTo(10.5f, 50.5f);
shapePath.Close();
//add free form
worksheet.Shapes.AddFreeform(1, 0, 1, 0, 300, 200, new ShapePath[] { shapePath });
Console.WriteLine("MoveTo method executed successfully with parameters (Single, Single)");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing LineTo method: {ex.Message}");
}
// Save the result
workbook.Save("ShapePathMethodMoveToWithSingleSingleDemo.xlsx");
}
}
}
```
### See Also
* class [ShapePath](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
