##DrawObjectEventHandler.Draw
DrawObjectEventHandler method. Implements this interface to get DrawObject and Bound when rendering
## DrawObjectEventHandler.Draw method
Implements this interface to get DrawObject and Bound when rendering.
```csharp
public virtual void Draw(DrawObject drawObject, float x, float y, float width, float height)
```
| Parameter | Type | Description |
| --- | --- | --- |
| drawObject | DrawObject | DrawObject will be initialized and returned when rendering |
| x | Single | Left of DrawObject |
| y | Single | Top of DrawObject |
| width | Single | Width of DrawObject |
| height | Single | Height of DrawObject |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Rendering;
using Aspose.Cells.Drawing;
using System;
public class DrawObjectEventHandlerMethodDrawWithDrawObjectSingleSingleSingleSiDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].Value = "Aspose.Cells Drawing Demo";
ImageOrPrintOptions options = new ImageOrPrintOptions();
options.ImageType = ImageType.Png;
options.DrawObjectEventHandler = new CustomDrawObjectEventHandler();
SheetRender sheetRender = new SheetRender(worksheet, options);
try
{
sheetRender.ToImage(0, "DrawDemoOutput.png");
Console.WriteLine("Draw method executed during rendering. Output saved to DrawDemoOutput.png");
}
catch (Exception ex)
{
Console.WriteLine($"Error during rendering: {ex.Message}");
}
}
private class CustomDrawObjectEventHandler : DrawObjectEventHandler
{
public override void Draw(DrawObject drawObject, float x, float y, float width, float height)
{
// This implementation will be called during rendering for each DrawObject
Console.WriteLine($"Drawn {drawObject.Type} at ({x:F1}, {y:F1}) [{width:F1}x{height:F1}]");
}
}
}
}
```
### See Also
* class [DrawObject](../../drawobject/)
* class [DrawObjectEventHandler](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)
