##Shape.IsDecorative
Shape property. Indicates whether the object is decorative
## Shape.IsDecorative property
Indicates whether the object is decorative.
```csharp
public bool IsDecorative { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ShapePropertyIsDecorativeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Add a rectangle shape
Shape shape = worksheet.Shapes.AddRectangle(10, 10, 100, 100, 0, 0);
// Set the shape as decorative
shape.IsDecorative = true;
// Save the workbook
string outputPath = "ShapeIsDecorativeDemo.xlsx";
workbook.Save(outputPath);
// Reload the workbook to verify the property
Workbook loadedWorkbook = new Workbook(outputPath);
Shape loadedShape = loadedWorkbook.Worksheets[0].Shapes[0];
// Output the result
Console.WriteLine("Shape IsDecorative property: " + loadedShape.IsDecorative);
}
}
}
```
### See Also
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
