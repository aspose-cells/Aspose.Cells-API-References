##PaginatedSaveOptions.PageCount
PaginatedSaveOptions property. Gets or sets the number of pages to save
## PaginatedSaveOptions.PageCount property
Gets or sets the number of pages to save.
```csharp
public int PageCount { get; set; }
```
### Remarks
Default is System.Int32.MaxValue which means all pages will be rendered..
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class PaginatedSaveOptionsPropertyPageCountDemo
{
public static void Run()
{
// Open an Excel file
Workbook wb = new Workbook("Book1.xlsx");
// Initialize PDF save options
PdfSaveOptions options = new PdfSaveOptions();
// Set to print only 2 pages starting from page 4 (0-based index 3)
options.PageIndex = 3;
options.PageCount = 2;
// Save the PDF file
wb.Save("output.pdf", options);
Console.WriteLine("PDF saved with selected pages.");
}
}
}
```
### See Also
* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
