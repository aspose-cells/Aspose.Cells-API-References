##Shape.MsoDrawingType
Shape property. Gets drawing type
## Shape.MsoDrawingType property
Gets drawing type.
```csharp
public MsoDrawingType MsoDrawingType { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ShapePropertyMsoDrawingTypeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a rectangle shape (corrected parameters)
Shape rectangle = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 50, 50);
// Get and display the MsoDrawingType of the shape
MsoDrawingType drawingType = rectangle.MsoDrawingType;
Console.WriteLine("Shape MsoDrawingType: " + drawingType.ToString());
// Add a line shape (corrected parameters)
Shape line = worksheet.Shapes.AddLine(3, 0, 3, 100, 150, 1);
// Get and display the MsoDrawingType of the line
drawingType = line.MsoDrawingType;
Console.WriteLine("Line MsoDrawingType: " + drawingType.ToString());
}
}
}
```
### See Also
* enum [MsoDrawingType](../../msodrawingtype/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
