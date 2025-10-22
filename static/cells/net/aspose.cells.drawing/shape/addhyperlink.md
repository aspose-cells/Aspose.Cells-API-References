##Shape.AddHyperlink
Shape method. Adds a hyperlink to the shape
## Shape.AddHyperlink method
Adds a hyperlink to the shape.
```csharp
public Hyperlink AddHyperlink(string address)
```
| Parameter | Type | Description |
| --- | --- | --- |
| address | String | Address of the hyperlink. |
### Return Value
Return the new hyperlink object.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ShapeMethodAddHyperlinkWithStringDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a shape to the worksheet
Shape shape = worksheet.Shapes.AddRectangle(1, 1, 100, 100, 0, 0);
// Add a hyperlink to the shape using string URL
Aspose.Cells.Hyperlink hyperlink = shape.AddHyperlink("https://www.aspose.com/");
// Save the workbook
workbook.Save("ShapeWithHyperlink.xlsx");
}
}
}
```
### See Also
* class [Hyperlink](../../../aspose.cells/hyperlink/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
