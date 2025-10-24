##ShapePath.Close
ShapePath method. Closes the current figure and starts a new figure. If the current figure contains a sequence of connected lines and curves the method closes the loop by connecting a line from the endpoint to the starting point
## ShapePath.Close method
Closes the current figure and starts a new figure. If the current figure contains a sequence of connected lines and curves, the method closes the loop by connecting a line from the endpoint to the starting point.
```csharp
public void Close()
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System;
public class ShapePathMethodCloseDemo
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
shapePath.MoveTo(60, 45);
shapePath.ArcTo(25, 25, 0, 270);
// Close the path
shapePath.Close();
shapePath.MoveTo(60, 20);
shapePath.LineTo(110, 70);
shapePath.LineTo(125, 155.5f);
shapePath.ArcTo(35.5f, 35.5f, 0, 270);
// Close the path
shapePath.Close();
//add free form
worksheet.Shapes.AddFreeform(1, 0, 1, 0, 300, 200, new ShapePath[] { shapePath });
Console.WriteLine("Close method called successfully to complete the shape path");
// Save the workbook
workbook.Save("ShapePathMethodCloseDemo.xlsx");
}
catch (Exception ex)
{
Console.WriteLine($"Error calling Close method: {ex.Message}");
}
}
}
}
```
### See Also
* class [ShapePath](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
