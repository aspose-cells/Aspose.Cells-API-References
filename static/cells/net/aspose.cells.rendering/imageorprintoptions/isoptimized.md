##ImageOrPrintOptions.IsOptimized
ImageOrPrintOptions property. Indicates whether to optimize the output elements
## ImageOrPrintOptions.IsOptimized property
Indicates whether to optimize the output elements.
```csharp
public bool IsOptimized { get; set; }
```
### Remarks
Default value is false. Currently when this property is set to true, the following optimizations will be done: 1. optimize the border lines. 2. optimize the file size while rendering to Svg image.
### Examples
```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Rendering;
namespace AsposeCellsExamples
{
public class ImageOrPrintOptionsPropertyIsOptimizedDemo
{
public static void Run()
{
// Create a workbook with sample data
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Add sample data to cells
for (int i = 0; i < 10; i++)
{
for (int j = 0; j < 5; j++)
{
sheet.Cells[i, j].PutValue($"Data {i}-{j}");
}
}
// Set up image rendering options
ImageOrPrintOptions options = new ImageOrPrintOptions();
options.ImageType = Aspose.Cells.Drawing.ImageType.Png;
options.OnePagePerSheet = true;
// Demonstrate IsOptimized property
options.IsOptimized = true; // Enable optimization
// Render the sheet to image
SheetRender renderer = new SheetRender(sheet, options);
MemoryStream stream = new MemoryStream();
renderer.ToImage(0, stream);
Console.WriteLine($"Image rendered with optimization: {options.IsOptimized}");
Console.WriteLine($"Image size: {stream.Length} bytes");
}
}
}
```
### See Also
* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)
