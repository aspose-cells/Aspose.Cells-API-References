##Shape.IsSmartArt
Shape property. Indicates whether the shape is a smart art
## Shape.IsSmartArt property
Indicates whether the shape is a smart art.
```csharp
public bool IsSmartArt { get; }
```
### Remarks
Only for ooxml file.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ShapePropertyIsSmartArtDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a SmartArt shape (Note: Aspose.Cells doesn't directly expose SmartArt creation in current versions)
// For demonstration, we'll check existing shapes
Shape shape = worksheet.Shapes.AddRectangle(1, 1, 100, 100, 0, 0);
// Check if the shape is SmartArt
if (shape.IsSmartArt)
{
Console.WriteLine("The shape is a SmartArt object");
}
else
{
Console.WriteLine("The shape is not a SmartArt object");
}
}
}
}
```
### See Also
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
