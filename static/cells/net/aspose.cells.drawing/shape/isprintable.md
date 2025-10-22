##Shape.IsPrintable
Shape property. Indicates whether the object is printable. If False this shape will not be printed when printing
## Shape.IsPrintable property
Indicates whether the object is printable. If False, this shape will not be printed when printing.
```csharp
public bool IsPrintable { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ShapePropertyIsPrintableDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a shape to the worksheet
Shape shape = worksheet.Shapes.AddRectangle(1, 1, 100, 100, 0, 0);
// Demonstrate IsPrintable property
Console.WriteLine("Shape is printable initially: " + shape.IsPrintable);
// Toggle the IsPrintable property
shape.IsPrintable = !shape.IsPrintable;
Console.WriteLine("Shape is printable after toggle: " + shape.IsPrintable);
// Set IsPrintable to false explicitly
shape.IsPrintable = false;
Console.WriteLine("Shape is printable after setting to false: " + shape.IsPrintable);
}
}
}
```
### See Also
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
