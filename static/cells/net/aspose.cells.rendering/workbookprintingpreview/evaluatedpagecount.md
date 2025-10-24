##WorkbookPrintingPreview.EvaluatedPageCount
WorkbookPrintingPreview property. Evaluate the total page count of this workbook
## WorkbookPrintingPreview.EvaluatedPageCount property
Evaluate the total page count of this workbook
```csharp
public int EvaluatedPageCount { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;
namespace AsposeCellsExamples
{
public class WorkbookPrintingPreviewPropertyEvaluatedPageCountDemo
{
public static void Run()
{
// Create a workbook with sample data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data to the worksheet
for (int i = 0; i < 100; i++)
{
worksheet.Cells[i, 0].PutValue("Row " + (i + 1));
}
// Create printing preview options
ImageOrPrintOptions options = new ImageOrPrintOptions();
// Create workbook printing preview
WorkbookPrintingPreview printingPreview = new WorkbookPrintingPreview(workbook, options);
// Get and display the evaluated page count
Console.WriteLine("Evaluated Page Count: " + printingPreview.EvaluatedPageCount);
}
}
}
```
### See Also
* class [WorkbookPrintingPreview](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)
