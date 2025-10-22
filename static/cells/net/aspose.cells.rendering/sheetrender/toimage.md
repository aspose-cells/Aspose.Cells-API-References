##SheetRender.ToImage
SheetRender method. Render certain page to a Graphics
## ToImage(int, Graphics, float, float, float, float) {#toimage_2}
Render certain page to a Graphics
```csharp
public void ToImage(int pageIndex, Graphics g, float x, float y, float width, float height)
```
| Parameter | Type | Description |
| --- | --- | --- |
| pageIndex | Int32 | indicate which page is to be converted |
| g | Graphics | The object where to render to. |
| x | Single | The X coordinate (in pixels) of the top left corner of the rendered page. |
| y | Single | The Y coordinate (in pixels) of the top left corner of the rendered page. |
| width | Single | The maximum width (in pixels) that can be occupied by the rendered page. |
| height | Single | The maximum height (in pixels) that can be occupied by the rendered page. |
### See Also
* class [SheetRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)
## ToImage(int, Graphics, float, float) {#toimage_1}
Render certain page to a Graphics
```csharp
public void ToImage(int pageIndex, Graphics g, float x, float y)
```
| Parameter | Type | Description |
| --- | --- | --- |
| pageIndex | Int32 | indicate which page is to be converted |
| g | Graphics | The object where to render to. |
| x | Single | The X coordinate (in pixels) of the top left corner of the rendered page. |
| y | Single | The Y coordinate (in pixels) of the top left corner of the rendered page. |
### See Also
* class [SheetRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)
## ToImage(int, string) {#toimage_4}
Render certain page to a file.
```csharp
public void ToImage(int pageIndex, string fileName)
```
| Parameter | Type | Description |
| --- | --- | --- |
| pageIndex | Int32 | indicate which page is to be converted |
| fileName | String | filename of the output image |
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;
namespace AsposeCellsExamples
{
public class SheetRenderMethodToImageWithInt32StringDemo
{
public static void Run()
{
// Load the source Excel file
Workbook workbook = new Workbook("Book1.xlsx");
// Create image options
ImageOrPrintOptions options = new ImageOrPrintOptions();
options.ImageType = Aspose.Cells.Drawing.ImageType.Png;
// Create sheet render for the first worksheet
SheetRender sheetRender = new SheetRender(workbook.Worksheets[0], options);
// Render the first page of the sheet to an image file
sheetRender.ToImage(0, "output.png");
Console.WriteLine("Sheet rendered to image successfully.");
}
}
}
```
### See Also
* class [SheetRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)
## ToImage(int, Stream) {#toimage_3}
Render certain page to a stream.
```csharp
public void ToImage(int pageIndex, Stream stream)
```
| Parameter | Type | Description |
| --- | --- | --- |
| pageIndex | Int32 | indicate which page is to be converted |
| stream | Stream | the stream of the output image |
### See Also
* class [SheetRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)
## ToImage(int) {#toimage}
Render certain page to a Bitmap object.
```csharp
public Bitmap ToImage(int pageIndex)
```
| Parameter | Type | Description |
| --- | --- | --- |
| pageIndex | Int32 | indicate which page is to be converted |
### Return Value
the bitmap object of the page
### See Also
* class [SheetRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)
