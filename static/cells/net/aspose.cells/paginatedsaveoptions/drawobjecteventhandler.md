##PaginatedSaveOptions.DrawObjectEventHandler
PaginatedSaveOptions property. Implements this interface to get DrawObject and Bound when rendering
## PaginatedSaveOptions.DrawObjectEventHandler property
Implements this interface to get DrawObject and Bound when rendering.
```csharp
public DrawObjectEventHandler DrawObjectEventHandler { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Rendering;
using System;
public class PaginatedSaveOptionsPropertyDrawObjectEventHandlerDemo
{
private class CustomDrawObjectEventHandler : DrawObjectEventHandler
{
public override void Draw(DrawObject drawObject, float x, float y, float width, float height)
{
Console.WriteLine($"DrawObject Type: {drawObject.Type}");
Console.WriteLine($"Position: X={x}, Y={y}, Width={width}, Height={height}");
}
}
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add some sample data and shapes
worksheet.Cells["A1"].PutValue("Test DrawObjectEventHandler");
worksheet.Cells["A2"].PutValue("This will demonstrate the event handler during rendering");
// Create a paginated save options instance
PdfSaveOptions saveOptions = new PdfSaveOptions();
// Display the current value of the property (should be null initially)
Console.WriteLine("Current DrawObjectEventHandler value: " + (saveOptions.DrawObjectEventHandler == null ? "null" : "assigned"));
// Set a new custom event handler
saveOptions.DrawObjectEventHandler = new CustomDrawObjectEventHandler();
// This will trigger the Draw method during rendering
workbook.Save("PropertyDrawObjectEventHandlerDemo.pdf", saveOptions);
// Change the event handler to null to demonstrate the difference
saveOptions.DrawObjectEventHandler = null;
workbook.Save("PropertyDrawObjectEventHandlerDemo_NoHandler.pdf", saveOptions);
}
}
}
```
### See Also
* class [DrawObjectEventHandler](../../../aspose.cells.rendering/drawobjecteventhandler/)
* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
