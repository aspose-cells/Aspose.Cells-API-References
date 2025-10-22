##PdfBookmarkEntry.Destination
PdfBookmarkEntry property. The cell to which the bookmark link
## PdfBookmarkEntry.Destination property
The cell to which the bookmark link.
```csharp
public Cell Destination { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;
namespace AsposeCellsExamples
{
public class PdfBookmarkEntryPropertyDestinationDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample content
worksheet.Cells["A1"].PutValue("Bookmark Destination");
// Configure PDF save options with bookmark
PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
PdfBookmarkEntry entry = new PdfBookmarkEntry();
entry.Text = "Sample Bookmark";
entry.Destination = worksheet.Cells["A1"]; // Demonstrate Destination property
entry.IsOpen = true;
pdfSaveOptions.Bookmark = entry;
// Save the PDF
workbook.Save("PdfBookmarkEntryPropertyDestinationDemo.pdf", pdfSaveOptions);
}
}
}
```
### See Also
* class [Cell](../../../aspose.cells/cell/)
* class [PdfBookmarkEntry](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)
