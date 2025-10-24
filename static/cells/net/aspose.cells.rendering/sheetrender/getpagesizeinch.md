##SheetRender.GetPageSizeInch
SheetRender method. Get page size in inch of output image
## SheetRender.GetPageSizeInch method
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
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class SheetRenderMethodGetPageSizeInchWithInt32Demo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
worksheet.PageSetup.PrintArea = "A1:D10";
worksheet.PageSetup.LeftMargin = 0;
worksheet.PageSetup.RightMargin = 0;
worksheet.PageSetup.TopMargin = 0;
worksheet.PageSetup.BottomMargin = 0;
ImageOrPrintOptions options = new ImageOrPrintOptions
{
OnePagePerSheet = true,
ImageType = ImageType.Png
};
SheetRender sheetRender = new SheetRender(worksheet, options);
float[] pageSize = sheetRender.GetPageSizeInch(0);
Console.WriteLine($"Page Size (Inches): Width={pageSize[0]}, Height={pageSize[1]}");
}
}
}
```
### See Also
* class [SheetRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)
