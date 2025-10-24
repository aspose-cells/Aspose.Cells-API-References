##WorkbookRender.WorkbookRender
WorkbookRender constructor. The construct of WorkbookRender
## WorkbookRender constructor
The construct of WorkbookRender
```csharp
public WorkbookRender(Workbook workbook, ImageOrPrintOptions options)
```
| Parameter | Type | Description |
| --- | --- | --- |
| workbook | Workbook | Indicate which workbook to be rendered. |
| options | ImageOrPrintOptions | ImageOrPrintOptions contains some property of output image |
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;
namespace AsposeCellsExamples
{
public class WorkbookRenderMethodctorWithWorkbookImageOrPrintOptionsDemo
{
public static void Run()
{
// Create a new workbook with sample data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue("Hello");
worksheet.Cells["B1"].PutValue("World");
// Create image/print options
ImageOrPrintOptions options = new ImageOrPrintOptions();
options.ImageType = Aspose.Cells.Drawing.ImageType.Png;
// Create workbook renderer
WorkbookRender renderer = new WorkbookRender(workbook, options);
// Output page count
Console.WriteLine("Total pages: " + renderer.PageCount);
}
}
}
```
### See Also
* class [Workbook](../../../aspose.cells/workbook/)
* class [ImageOrPrintOptions](../../imageorprintoptions/)
* class [WorkbookRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)
