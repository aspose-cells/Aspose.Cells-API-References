##Shape.Id
Shape property. Gets the identifier of this shape
## Shape.Id property
Gets the identifier of this shape.
```csharp
public int Id { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ShapePropertyIdDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a shape to the worksheet
Shape shape = worksheet.Shapes.AddRectangle(1, 1, 100, 100, 0, 0);
// Get and display the shape's ID
int id = shape.Id;
Console.WriteLine("Shape ID: " + id);
// Modify the shape's properties
shape.Name = "Rectangle1";
shape.Text = "Shape with ID: " + id;
// Save the workbook
workbook.Save("ShapePropertyIdDemo.xlsx");
}
}
}
```
### See Also
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
