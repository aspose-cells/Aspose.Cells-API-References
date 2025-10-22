##Shape.Hyperlink
Shape property. Gets the hyperlink of the shape
## Shape.Hyperlink property
Gets the hyperlink of the shape.
```csharp
public Hyperlink Hyperlink { get; }
```
### Examples
```csharp
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class ShapePropertyHyperlinkDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
Aspose.Cells.Drawing.Shape shape = sheet.Shapes.AddRectangle(0, 0, 10, 10, 100, 150);
Hyperlink hyperlink = shape.Hyperlink;
hyperlink.Address = "https://www.aspose.com";
hyperlink.ScreenTip = "Click to open Aspose website";
workbook.Save("ShapeHyperlinkDemo.xlsx");
}
}
}
```
### See Also
* class [Hyperlink](../../../aspose.cells/hyperlink/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
