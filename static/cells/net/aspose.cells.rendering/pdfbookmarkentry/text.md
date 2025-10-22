##PdfBookmarkEntry.Text
PdfBookmarkEntry property. Title of a bookmark
## PdfBookmarkEntry.Text property
Title of a bookmark.
```csharp
public string Text { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;
namespace AsposeCellsExamples
{
public class PdfBookmarkEntryPropertyTextDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample content
worksheet.Cells["A1"].PutValue("Page 1 Content");
// Create PDF bookmark entry
PdfBookmarkEntry entry = new PdfBookmarkEntry();
entry.Text = "Section 1"; // Demonstrating Text property usage
entry.Destination = worksheet.Cells["A1"];
entry.IsOpen = true;
// Set save options with bookmark
PdfSaveOptions saveOptions = new PdfSaveOptions();
saveOptions.Bookmark = entry;
// Save the workbook with bookmark
workbook.Save("output.pdf", saveOptions);
Console.WriteLine("PDF with bookmark created successfully.");
}
}
}
```
### See Also
* class [PdfBookmarkEntry](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)
