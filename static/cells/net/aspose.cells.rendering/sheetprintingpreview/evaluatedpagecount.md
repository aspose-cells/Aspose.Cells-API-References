##SheetPrintingPreview.EvaluatedPageCount
SheetPrintingPreview property. Evaluate the total page count of this worksheet
## SheetPrintingPreview.EvaluatedPageCount property
Evaluate the total page count of this worksheet
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
public class SheetPrintingPreviewPropertyEvaluatedPageCountDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data to the worksheet
for (int i = 0; i < 100; i++)
{
worksheet.Cells[i, 0].Value = "Row " + (i + 1);
}
ImageOrPrintOptions options = new ImageOrPrintOptions();
SheetPrintingPreview preview = new SheetPrintingPreview(worksheet, options);
Console.WriteLine("Evaluated Page Count: " + preview.EvaluatedPageCount);
}
}
}
```
### See Also
* class [SheetPrintingPreview](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)
