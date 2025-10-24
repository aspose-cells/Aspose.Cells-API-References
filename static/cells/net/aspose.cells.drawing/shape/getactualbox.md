##Shape.GetActualBox
Shape method. Get the actual position and size of the shape after applying rotation flip etc
## Shape.GetActualBox method
Get the actual position and size of the shape (after applying rotation, flip, etc.)
```csharp
public float[] GetActualBox()
```
### Return Value
Return the position and size in the order of x, y, w, h
### Remarks
Note:The interface is not fully functional, especially the location information is not correct.It is recommended not to use this interface until the function is complete.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ShapeMethodGetActualBoxDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a rectangle shape
Shape rectangle = worksheet.Shapes.AddRectangle(10, 10, 100, 80, 0, 0);
// Get the actual box dimensions of the shape
float[] box = rectangle.GetActualBox();
// Output the box dimensions
Console.WriteLine("Actual Box Dimensions:");
Console.WriteLine($"Left: {box[0]}");
Console.WriteLine($"Top: {box[1]}");
Console.WriteLine($"Right: {box[2]}");
Console.WriteLine($"Bottom: {box[3]}");
// Save the workbook
workbook.Save("ShapeGetActualBoxDemo.xlsx");
}
}
}
```
### See Also
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
