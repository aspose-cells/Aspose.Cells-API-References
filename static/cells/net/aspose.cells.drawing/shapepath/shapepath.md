##ShapePath.ShapePath
ShapePath constructor. Initializes a new instance of the ShapePath class
## ShapePath constructor
Initializes a new instance of the [`ShapePath`](../) class.
```csharp
public ShapePath()
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System;
public class ShapePathMethodCtorDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
try
{
// Create a new shape path using the #ctor method
ShapePath shapePath = new ShapePath();
// Add path segments to create a simple shape
shapePath.MoveTo(100, 100);
shapePath.LineTo(200, 100);
shapePath.LineTo(200, 200);
shapePath.LineTo(100, 200);
shapePath.Close();
//add free form
worksheet.Shapes.AddFreeform(1, 0, 1, 0, 200, 200, new ShapePath[] { shapePath });
Console.WriteLine("ShapePath created and added to worksheet successfully");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing ShapePath constructor: {ex.Message}");
}
// Save the result
workbook.Save("ShapePathMethodCtorDemo.xlsx");
}
}
}
```
### See Also
* class [ShapePath](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
