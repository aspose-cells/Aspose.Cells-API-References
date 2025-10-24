##Shape.CreateId
Shape property. Gets and sets create id for this shape
## Shape.CreateId property
Gets and sets create id for this shape.
```csharp
public Guid CreateId { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ShapePropertyCreateIdDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Add a rectangle shape
Shape shape = worksheet.Shapes.AddRectangle(10, 10, 100, 100, 200, 150);
// Create and assign a new GUID as CreateId
Guid createId = Guid.NewGuid();
shape.CreateId = createId;
// Save the workbook
workbook.Save("ShapeCreateIdDemo.xlsx");
// Reload the workbook to verify the CreateId persists
Workbook loadedWorkbook = new Workbook("ShapeCreateIdDemo.xlsx");
Shape loadedShape = loadedWorkbook.Worksheets[0].Shapes[0];
// Output the CreateId for verification
Console.WriteLine("Original CreateId: " + createId);
Console.WriteLine("Loaded CreateId: " + loadedShape.CreateId);
}
}
}
```
### See Also
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
