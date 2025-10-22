##SheetRender.ToTiff
SheetRender method. Render whole worksheet as Tiff Image to stream
## ToTiff(Stream) {#totiff}
Render whole worksheet as Tiff Image to stream.
```csharp
public void ToTiff(Stream stream)
```
| Parameter | Type | Description |
| --- | --- | --- |
| stream | Stream | the stream of the output image |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Rendering;
using System;
using System.IO;
public class SheetRenderMethodToTiffWithStreamDemo
{
public static void Run()
{
// Create a new workbook and access first worksheet
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample content to demonstrate rendering
worksheet.Cells["A1"].PutValue("Aspose.Cells TIFF Rendering Demo");
// Configure image options for rendering
ImageOrPrintOptions options = new ImageOrPrintOptions();
options.OnePagePerSheet = true;
// Create sheet renderer with configured options
SheetRender renderer = new SheetRender(worksheet, options);
try
{
// Create output stream for TIFF image
using (FileStream tiffStream = new FileStream("output.tiff", FileMode.Create))
{
// Render worksheet to TIFF using stream
renderer.ToTiff(tiffStream);
Console.WriteLine("Worksheet successfully rendered to TIFF stream.");
}
}
catch (Exception ex)
{
Console.WriteLine($"Error during TIFF rendering: {ex.Message}");
}
}
}
}
```
### See Also
* class [SheetRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)
## ToTiff(string) {#totiff_1}
Render whole worksheet as Tiff Image to a file.
```csharp
public void ToTiff(string filename)
```
| Parameter | Type | Description |
| --- | --- | --- |
| filename | String | the filename of the output image |
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;
namespace AsposeCellsExamples
{
public class SheetRenderMethodToTiffWithStringDemo
{
public static void Run()
{
// Load the source Excel file
Workbook workbook = new Workbook("Book1.xlsx");
// Create image or print options
ImageOrPrintOptions options = new ImageOrPrintOptions();
options.SaveFormat = SaveFormat.Tiff;
// Create sheet render for the first worksheet
SheetRender sheetRender = new SheetRender(workbook.Worksheets[0], options);
// Save all pages of the sheet as a multi-page TIFF file
sheetRender.ToTiff("output.tiff");
}
}
}
```
### See Also
* class [SheetRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)
