##WorkbookRender.PageCount
WorkbookRender property. Gets the total page count of workbook
## WorkbookRender.PageCount property
Gets the total page count of workbook.
```csharp
public int PageCount { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;
namespace AsposeCellsExamples
{
public class WorkbookRenderPropertyPageCountDemo
{
public static void Run()
{
// Create a new workbook with sample data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue("Page 1 Content");
// Add a second worksheet
workbook.Worksheets.Add();
worksheet = workbook.Worksheets[1];
worksheet.Cells["A1"].PutValue("Page 2 Content");
// Create render options and workbook renderer
ImageOrPrintOptions options = new ImageOrPrintOptions
{
OnePagePerSheet = true
};
WorkbookRender renderer = new WorkbookRender(workbook, options);
// Demonstrate PageCount usage
Console.WriteLine($"Total pages to render: {renderer.PageCount}");
// Render each page to image
for (int i = 0; i < renderer.PageCount; i++)
{
string outputPath = $"Page_{i}.png";
renderer.ToImage(i, outputPath);
Console.WriteLine($"Rendered page {i+1} to {outputPath}");
}
}
}
}
```
### See Also
* class [WorkbookRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)
