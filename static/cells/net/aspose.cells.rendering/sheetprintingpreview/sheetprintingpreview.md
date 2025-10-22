##SheetPrintingPreview.SheetPrintingPreview
SheetPrintingPreview constructor. The construct of SheetPrintingPreview
## SheetPrintingPreview constructor
The construct of SheetPrintingPreview
```csharp
public SheetPrintingPreview(Worksheet sheet, ImageOrPrintOptions options)
```
| Parameter | Type | Description |
| --- | --- | --- |
| sheet | Worksheet | Indicate which spreadsheet to be printed. |
| options | ImageOrPrintOptions | ImageOrPrintOptions contains some property of output |
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;
namespace AsposeCellsExamples
{
public class SheetPrintingPreviewMethodctorWithWorksheetImageOrPrintOptionsDemo
{
public static void Run()
{
// Create a workbook with sample data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data to worksheet
for (int i = 0; i < 10; i++)
{
for (int j = 0; j < 5; j++)
{
worksheet.Cells[i, j].PutValue($"Data {i},{j}");
}
}
// Create image/print options
ImageOrPrintOptions options = new ImageOrPrintOptions();
options.PrintingPage = PrintingPageType.Default;
// Create sheet printing preview
SheetPrintingPreview preview = new SheetPrintingPreview(worksheet, options);
// Output the evaluated page count
Console.WriteLine($"Evaluated page count: {preview.EvaluatedPageCount}");
}
}
}
```
### See Also
* class [Worksheet](../../../aspose.cells/worksheet/)
* class [ImageOrPrintOptions](../../imageorprintoptions/)
* class [SheetPrintingPreview](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)
