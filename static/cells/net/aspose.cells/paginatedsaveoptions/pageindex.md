##PaginatedSaveOptions.PageIndex
PaginatedSaveOptions property. Gets or sets the 0based index of the first page to save
## PaginatedSaveOptions.PageIndex property
Gets or sets the 0-based index of the first page to save.
```csharp
public int PageIndex { get; set; }
```
### Remarks
Default is 0.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class PaginatedSaveOptionsPropertyPageIndexDemo
{
public static void Run()
{
// Create a new workbook with sample data
Workbook wb = new Workbook();
Worksheet sheet = wb.Worksheets[0];
// Add sample data across multiple pages
for (int i = 0; i < 100; i++)
{
sheet.Cells[i, 0].Value = "Data " + (i + 1);
}
// Set PDF save options
PdfSaveOptions options = new PdfSaveOptions();
// Set to print pages 3-4 (0-based index)
options.PageIndex = 2;  // Third page (index 2)
options.PageCount = 2; // Print 2 pages
// Save the PDF with selected pages
wb.Save("SelectedPages.pdf", options);
Console.WriteLine("PDF with pages 3-4 created successfully.");
}
}
}
```
### See Also
* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
