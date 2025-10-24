##WorkbookRender.GetPageSizeInch
WorkbookRender method. Get page size in inch of output image
## WorkbookRender.GetPageSizeInch method
Get page size in inch of output image.
```csharp
public float[] GetPageSizeInch(int pageIndex)
```
| Parameter | Type | Description |
| --- | --- | --- |
| pageIndex | Int32 | The page index is based on zero. |
### Return Value
Page size of image, [0] for width and [1] for height
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;
namespace AsposeCellsExamples
{
public class WorkbookRenderMethodGetPageSizeInchWithInt32Demo
{
public static void Run()
{
Workbook wb = new Workbook();
Worksheet sheet = wb.Worksheets[0];
sheet.Cells["A1"].PutValue("Test page size");
sheet.PageSetup.PaperSize = PaperSizeType.PaperLetter;
ImageOrPrintOptions imgOpt = new ImageOrPrintOptions();
WorkbookRender wr = new WorkbookRender(wb, imgOpt);
float[] pageSize = wr.GetPageSizeInch(0);
Console.WriteLine($"Page size in inches: {pageSize[0]} x {pageSize[1]}");
}
}
}
```
### See Also
* class [WorkbookRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)
