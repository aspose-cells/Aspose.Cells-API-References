##Worksheet.GetPrintingPageBreaks
Worksheet method. Gets automatic page breaks
## Worksheet.GetPrintingPageBreaks method
Gets automatic page breaks.
```csharp
public CellArea[] GetPrintingPageBreaks(ImageOrPrintOptions options)
```
| Parameter | Type | Description |
| --- | --- | --- |
| options | ImageOrPrintOptions | The print options |
### Return Value
The automatic page breaks areas.
### Remarks
Each cell area represents a paper.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;
namespace AsposeCellsExamples
{
public class WorksheetMethodGetPrintingPageBreaksWithImageOrPrintOptionsDemo
{
public static void Run()
{
// Create a workbook with sample data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data to create page breaks
for (int i = 0; i < 100; i++)
{
worksheet.Cells[$"A{i+1}"].PutValue($"Row {i+1}");
}
// Set print area and page setup
worksheet.PageSetup.PrintArea = "A1:A100";
worksheet.PageSetup.FitToPagesTall = 1;
worksheet.PageSetup.FitToPagesWide = 1;
// Get page breaks with ImageOrPrintOptions
ImageOrPrintOptions options = new ImageOrPrintOptions();
CellArea[] pageBreaks = worksheet.GetPrintingPageBreaks(options);
// Output the first page break information
Console.WriteLine($"First page break ends at row: {pageBreaks[0].EndRow}");
}
}
}
```
### See Also
* struct [CellArea](../../cellarea/)
* class [ImageOrPrintOptions](../../../aspose.cells.rendering/imageorprintoptions/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
