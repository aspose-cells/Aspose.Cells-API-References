##Shape.Title
Shape property. Specifies the title caption of the current shape object
## Shape.Title property
Specifies the title (caption) of the current shape object.
```csharp
public string Title { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ShapePropertyTitleDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a rectangle shape with all required parameters
Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 1, 100, 200);
// Set the title of the shape
shape.Title = "title1";
// Verify the title was set
Console.WriteLine("Shape title: " + shape.Title);
}
}
}
```
### See Also
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
