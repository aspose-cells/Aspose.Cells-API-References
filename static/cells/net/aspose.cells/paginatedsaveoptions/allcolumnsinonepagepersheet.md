##PaginatedSaveOptions.AllColumnsInOnePagePerSheet
PaginatedSaveOptions property. If AllColumnsInOnePagePerSheet is true  all column content of one sheet will output to only one page in result. The width of paper size of pagesetup will be ignored and the other settings of pagesetup will still take effect
## PaginatedSaveOptions.AllColumnsInOnePagePerSheet property
If AllColumnsInOnePagePerSheet is true , all column content of one sheet will output to only one page in result. The width of paper size of pagesetup will be ignored, and the other settings of pagesetup will still take effect.
```csharp
public bool AllColumnsInOnePagePerSheet { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class PaginatedSaveOptionsPropertyAllColumnsInOnePagePerSheetDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data to demonstrate column fitting
for (int i = 0; i < 50; i++)
{
worksheet.Cells[0, i].PutValue("Column " + (i + 1));
worksheet.Cells[1, i].PutValue("Sample data " + (i + 1));
}
// Create PDF save options
PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
pdfSaveOptions.OnePagePerSheet = true;
pdfSaveOptions.AllColumnsInOnePagePerSheet = true;
// Save the workbook with the options
workbook.Save("output.pdf", pdfSaveOptions);
Console.WriteLine("PDF saved with all columns in one page per sheet.");
}
}
}
```
### See Also
* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
