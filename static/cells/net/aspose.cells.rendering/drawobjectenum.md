##Enum DrawObjectEnum
Aspose.Cells.Rendering.DrawObjectEnum enum. Indicate Cell or Image of DrawObject
## DrawObjectEnum enumeration
Indicate Cell or Image of DrawObject.
```csharp
public enum DrawObjectEnum
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| Image | `0` | Indicate DrawObject is an Image |
| Cell | `1` | indicate DrawObject is an Cell |
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;
namespace AsposeCellsExamples
{
public class RenderingClassDrawObjectEnumDemo
{
public static void Run()
{
// Create a workbook and add sample data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue("Test Cell");
// Create a PdfSaveOptions object
PdfSaveOptions saveOptions = new PdfSaveOptions();
// Create a custom DrawObjectEventHandler
saveOptions.DrawObjectEventHandler = new CustomDrawObjectEventHandler();
// Save the workbook to PDF with the custom handler
workbook.Save("output.pdf", saveOptions);
}
}
public class CustomDrawObjectEventHandler : DrawObjectEventHandler
{
public override void Draw(DrawObject drawObject, float x, float y, float width, float height)
{
// Check if the draw object is a cell
if (drawObject.Type == DrawObjectEnum.Cell)
{
Cell cell = drawObject.Cell;
// Output cell information
Console.WriteLine($"Drawing Cell - Row: {cell.Row}, Column: {cell.Column}");
Console.WriteLine($"Position: ({x}, {y}), Size: {width}x{height}");
// Special handling for cell A1
if (cell.Row == 0 && cell.Column == 0)
{
Console.WriteLine("This is cell A1");
}
}
}
}
}
```
### See Also
* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)
