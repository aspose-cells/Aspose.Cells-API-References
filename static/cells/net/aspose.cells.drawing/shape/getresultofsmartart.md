##Shape.GetResultOfSmartArt
Shape method. Converting smart art to grouped shapes
## Shape.GetResultOfSmartArt method
Converting smart art to grouped shapes.
```csharp
public virtual GroupShape GetResultOfSmartArt()
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ShapeMethodGetResultOfSmartArtDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a rectangle shape (since we can't create SmartArt directly)
Shape shape = worksheet.Shapes.AddRectangle(0, 0, 200, 200, 0, 0);
// In a real scenario, we would load an existing SmartArt shape
// For demo purposes, we'll skip the IsSmartArt check since we can't set it
// Get result of SmartArt (would only work if shape was actually SmartArt)
GroupShape groupShape = shape.GetResultOfSmartArt();
Console.WriteLine("Converted shape to GroupShape");
}
}
}
```
### See Also
* class [GroupShape](../../groupshape/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
