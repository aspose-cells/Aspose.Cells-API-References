##PaginatedSaveOptions.OnePagePerSheet
PaginatedSaveOptions property. If OnePagePerSheet is true  all content of one sheet will output to only one page in result. The paper size of pagesetup will be invalid and the other settings of pagesetup will still take effect
## PaginatedSaveOptions.OnePagePerSheet property
If OnePagePerSheet is true , all content of one sheet will output to only one page in result. The paper size of pagesetup will be invalid, and the other settings of pagesetup will still take effect.
```csharp
public bool OnePagePerSheet { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class PaginatedSaveOptionsPropertyOnePagePerSheetDemo
{
public static void Run()
{
// Create a sample workbook with test data
Workbook workbook = new Workbook();
Worksheet sheet1 = workbook.Worksheets[0];
Worksheet sheet2 = workbook.Worksheets.Add("Sheet2");
// Add some sample data to both sheets
for (int i = 0; i < 10; i++)
{
sheet1.Cells[i, 0].Value = $"Sheet1 Data {i + 1}";
sheet2.Cells[i, 0].Value = $"Sheet2 Data {i + 1}";
}
// Set PDF save options with OnePagePerSheet
PdfSaveOptions options = new PdfSaveOptions();
options.OnePagePerSheet = true;
// Save the workbook to PDF
workbook.Save("output.pdf", options);
}
}
}
```
### See Also
* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
