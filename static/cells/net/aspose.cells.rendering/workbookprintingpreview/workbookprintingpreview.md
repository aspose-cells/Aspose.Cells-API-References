##WorkbookPrintingPreview.WorkbookPrintingPreview
WorkbookPrintingPreview constructor. The construct of WorkbookPrintingPreview
## WorkbookPrintingPreview constructor
The construct of WorkbookPrintingPreview
```csharp
public WorkbookPrintingPreview(Workbook workbook, ImageOrPrintOptions options)
```
| Parameter | Type | Description |
| --- | --- | --- |
| workbook | Workbook | Indicate which workbook to be printed. |
| options | ImageOrPrintOptions | ImageOrPrintOptions contains some property of output |
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;
namespace AsposeCellsExamples
{
public class WorkbookPrintingPreviewMethodCtorWithWorkbookImageOrPrintOptionsDemo
{
public static void Run()
{
// Create a new workbook with sample data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue("Test Printing Preview");
// Set print options
ImageOrPrintOptions options = new ImageOrPrintOptions();
options.PrintingPage = PrintingPageType.Default;
// Create printing preview with workbook and options
WorkbookPrintingPreview preview = new WorkbookPrintingPreview(workbook, options);
// Display page count
Console.WriteLine("Total pages: " + preview.EvaluatedPageCount);
}
}
}
```
### See Also
* class [Workbook](../../../aspose.cells/workbook/)
* class [ImageOrPrintOptions](../../imageorprintoptions/)
* class [WorkbookPrintingPreview](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)
