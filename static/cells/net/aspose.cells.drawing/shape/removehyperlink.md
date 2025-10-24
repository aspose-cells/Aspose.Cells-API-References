##Shape.RemoveHyperlink
Shape method. Removes the hyperlink of the shape
## Shape.RemoveHyperlink method
Removes the hyperlink of the shape.
```csharp
public void RemoveHyperlink()
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ShapeMethodRemoveHyperlinkDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a shape and set hyperlink
Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 50, 50);
shape.AddHyperlink("https://www.aspose.com");
// Remove the hyperlink
shape.RemoveHyperlink();
// Verify hyperlink is removed
Console.WriteLine("Hyperlink removed: " + (shape.Hyperlink == null));
// Save the workbook
workbook.Save("ShapeRemoveHyperlinkDemo.xlsx");
}
}
}
```
### See Also
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
