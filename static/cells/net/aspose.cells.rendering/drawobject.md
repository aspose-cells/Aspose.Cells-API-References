##Class DrawObject
Aspose.Cells.Rendering.DrawObject class. DrawObject will be initialized and returned when rendering
## DrawObject class
DrawObject will be initialized and returned when rendering.
```csharp
public class DrawObject
```
## Properties
| Name | Description |
| --- | --- |
| [Cell](../../aspose.cells.rendering/drawobject/cell/) { get; } | Indicates the Cell object when rendering. All properties of cell can be accessed. |
| [CurrentPage](../../aspose.cells.rendering/drawobject/currentpage/) { get; } | Indicates the page index of DrawObject. Page index is based on zero. One Sheet contains several pages when rendering. |
| [ImageBytes](../../aspose.cells.rendering/drawobject/imagebytes/) { get; } | Indicates image bytes of rendered Chart, Shape when rendering. |
| [Shape](../../aspose.cells.rendering/drawobject/shape/) { get; } | Indicates the Shape object when rendering. All properties of shape can be accessed. |
| [SheetIndex](../../aspose.cells.rendering/drawobject/sheetindex/) { get; } | Indicates current sheet index of DrawObject. |
| [TotalPages](../../aspose.cells.rendering/drawobject/totalpages/) { get; } | Indicates total pages in current rendering. |
| [Type](../../aspose.cells.rendering/drawobject/type/) { get; } | Indicates the type of DrawObject. |
### Examples
```csharp
using Aspose.Cells;
using Aspose.Cells.Rendering;
using System;
namespace AsposeCellsExamples
{
// Custom implementation of DrawObjectEventHandler
public class CustomDrawObjectEventHandler : DrawObjectEventHandler
{
public override void Draw(DrawObject drawObject, float x, float y, float width, float height)
{
Console.WriteLine($"Drawing object at X: {x}, Y: {y}, Width: {width}, Height: {height}");
Console.WriteLine($"Object Type: {drawObject.Type}");
Console.WriteLine($"Sheet Index: {drawObject.SheetIndex}, Current Page: {drawObject.CurrentPage}, Total Pages: {drawObject.TotalPages}");
if (drawObject.Cell != null)
{
Console.WriteLine($"Rendering Cell: {drawObject.Cell.Name}, Value: {drawObject.Cell.Value}");
}
if (drawObject.Shape != null)
{
Console.WriteLine($"Rendering Shape: {drawObject.Shape.Name}");
}
}
}
public class DrawObjectDemo
{
public static void RunDemo()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Add some sample data
sheet.Cells["A1"].PutValue("Hello");
sheet.Cells["A2"].PutValue("World");
sheet.Cells["A3"].Formula = "=A1 & \" \" & A2";
// Add a shape
Aspose.Cells.Drawing.Shape shape = sheet.Shapes.AddShape(Aspose.Cells.Drawing.MsoDrawingType.Rectangle, 5, 0, 5, 0, 100, 100);
shape.Text = "Sample Shape";
// Create an instance of CustomDrawObjectEventHandler
CustomDrawObjectEventHandler drawObjectEventHandler = new CustomDrawObjectEventHandler();
// Set image or print options
ImageOrPrintOptions options = new ImageOrPrintOptions
{
DrawObjectEventHandler = drawObjectEventHandler,
OnePagePerSheet = true,
ImageType = Aspose.Cells.Drawing.ImageType.Png
};
// Render the sheet to an image
SheetRender sr = new SheetRender(sheet, options);
sr.ToImage(0, "DrawObjectDemo.png");
// Save the workbook
workbook.Save("DrawObjectDemo.xlsx");
workbook.Save("DrawObjectDemo.pdf");
}
}
}
```
### See Also
* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)
