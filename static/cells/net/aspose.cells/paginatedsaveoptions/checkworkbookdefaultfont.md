##PaginatedSaveOptions.CheckWorkbookDefaultFont
PaginatedSaveOptions property. When characters in the Excel are Unicode and not be set with correct font in cell style They may appear as block in pdfimage. Set this to true to try to use workbooks default font to show these characters first
## PaginatedSaveOptions.CheckWorkbookDefaultFont property
When characters in the Excel are Unicode and not be set with correct font in cell style, They may appear as block in pdf,image. Set this to true to try to use workbook's default font to show these characters first.
```csharp
public bool CheckWorkbookDefaultFont { get; set; }
```
### Remarks
Default is true.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class PaginatedSaveOptionsPropertyCheckWorkbookDefaultFontDemo
{
public static void Run()
{
// Create a sample workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue("Test Content");
// Configure PDF save options
PdfSaveOptions saveOptions = new PdfSaveOptions();
saveOptions.CheckWorkbookDefaultFont = false;
// Save to PDF
workbook.Save("output.pdf", saveOptions);
Console.WriteLine("PDF saved with CheckWorkbookDefaultFont set to false");
}
}
}
```
### See Also
* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
