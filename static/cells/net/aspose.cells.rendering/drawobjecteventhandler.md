##Class DrawObjectEventHandler
Aspose.Cells.Rendering.DrawObjectEventHandler class. Interface to get DrawObject and Bound when rendering
## DrawObjectEventHandler class
Interface to get DrawObject and Bound when rendering.
```csharp
public abstract class DrawObjectEventHandler
```
## Methods
| Name | Description |
| --- | --- |
| virtual [Draw](../../aspose.cells.rendering/drawobjecteventhandler/draw/)(DrawObject, float, float, float, float) | Implements this interface to get DrawObject and Bound when rendering. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Rendering;
using System;
public class RenderingClassDrawObjectEventHandlerDemo
{
public static void Run()
{
// Create a new workbook with sample data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue("Sample Text");
worksheet.Cells["B2"].PutValue(12345);
worksheet.Shapes.AddRectangle(5, 5, 50, 100, 200, 300); // Added missing parameter
// Create PDF save options with custom render handler
PdfSaveOptions saveOptions = new PdfSaveOptions();
saveOptions.DrawObjectEventHandler = new CustomDrawObjectHandler();
// Save workbook to PDF with rendering customization
workbook.Save("DrawObjectEventHandlerDemo.pdf", saveOptions);
}
}
public class CustomDrawObjectHandler : DrawObjectEventHandler
{
public override void Draw(DrawObject drawObject, float x, float y, float width, float height)
{
// Demonstrate handling different render object types
switch (drawObject.Type)
{
case DrawObjectEnum.Cell:
Console.WriteLine($"Rendering cell at ({x}, {y})");
break;
case DrawObjectEnum.Image:
Console.WriteLine($"Rendering image at ({x}, {y})");
break;
}
}
}
}
```
### See Also
* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)
