##Shape.IsTextWrapped
Shape property. Gets and sets the text wrapped type of the shape which contains text
## Shape.IsTextWrapped property
Gets and sets the text wrapped type of the shape which contains text.
```csharp
public bool IsTextWrapped { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ShapePropertyIsTextWrappedDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a shape and set some text
Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 200, 0);
shape.Text = "This is a sample text that will demonstrate text wrapping functionality";
// Demonstrate IsTextWrapped property
Console.WriteLine("Initial IsTextWrapped value: " + shape.IsTextWrapped);
// Toggle the text wrapping
shape.IsTextWrapped = !shape.IsTextWrapped;
Console.WriteLine("After toggle, IsTextWrapped value: " + shape.IsTextWrapped);
// Save the workbook
workbook.Save("ShapeTextWrappingDemo.xlsx");
}
}
}
```
### See Also
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
