##ImageOrPrintOptions.DrawObjectEventHandler
ImageOrPrintOptions property. Implements this interface to get DrawObject and Bound when rendering
## ImageOrPrintOptions.DrawObjectEventHandler property
Implements this interface to get DrawObject and Bound when rendering.
```csharp
public DrawObjectEventHandler DrawObjectEventHandler { get; set; }
```
### Examples
```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Rendering;
namespace AsposeCellsExamples
{
public class ImageOrPrintOptionsPropertyDrawObjectEventHandlerDemo
{
public static void Run()
{
// Create a workbook with sample data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue("Hello");
worksheet.Cells["B1"].PutValue("World");
worksheet.Cells["A2"].PutValue(123);
worksheet.Cells["B2"].PutValue(456);
// Create custom DrawObject event handler
var drawHandler = new CustomDrawObjectEventHandler();
// Set image options with the event handler
ImageOrPrintOptions options = new ImageOrPrintOptions();
options.DrawObjectEventHandler = drawHandler;
// Render the worksheet to trigger the events
SheetRender render = new SheetRender(worksheet, options);
for (int pageIndex = 0; pageIndex < render.PageCount; pageIndex++)
{
using (MemoryStream stream = new MemoryStream())
{
render.ToImage(pageIndex, stream);
}
}
}
}
public class CustomDrawObjectEventHandler : DrawObjectEventHandler
{
public override void Draw(DrawObject drawObject, float x, float y, float width, float height)
{
// Example: Print information about the drawn object
Console.WriteLine($"Drawing {drawObject.Type} at ({x},{y}) with size {width}x{height}");
}
}
}
```
### See Also
* class [DrawObjectEventHandler](../../drawobjecteventhandler/)
* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)
