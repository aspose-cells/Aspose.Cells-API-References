##PdfSaveOptions.Bookmark
PdfSaveOptions property. Gets and sets the PdfBookmarkEntry object
## PdfSaveOptions.Bookmark property
Gets and sets the [`PdfBookmarkEntry`](../../../aspose.cells.rendering/pdfbookmarkentry/) object.
```csharp
public PdfBookmarkEntry Bookmark { get; set; }
```
### Examples
```csharp
using System;
using System.Collections;
using Aspose.Cells;
using Aspose.Cells.Rendering;
namespace AsposeCellsExamples
{
public class PdfSaveOptionsPropertyBookmarkDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Add three worksheets
Worksheet sheet1 = workbook.Worksheets.Add("Sheet1");
Worksheet sheet2 = workbook.Worksheets.Add("Sheet2");
Worksheet sheet3 = workbook.Worksheets.Add("Sheet3");
// Set values in cells that will be bookmark destinations
sheet1.Cells["A1"].Value = "Sheet1 Content";
sheet2.Cells["A1"].Value = "Sheet2 Content";
sheet3.Cells["A1"].Value = "Sheet3 Content";
// Create root bookmark
PdfBookmarkEntry rootBookmark = new PdfBookmarkEntry
{
Text = "Root",
Destination = sheet1.Cells["A1"],
IsOpen = true
};
// Create sub-bookmarks
PdfBookmarkEntry subBookmark1 = new PdfBookmarkEntry
{
Text = "Sheet2",
Destination = sheet2.Cells["A1"]
};
PdfBookmarkEntry subBookmark2 = new PdfBookmarkEntry
{
Text = "Sheet3",
Destination = sheet3.Cells["A1"]
};
// Add sub-bookmarks to root
rootBookmark.SubEntry = new ArrayList { subBookmark1, subBookmark2 };
// Configure PDF save options with bookmarks
PdfSaveOptions options = new PdfSaveOptions
{
Bookmark = rootBookmark
};
// Save to memory stream (could save to file in real usage)
workbook.Save("output.pdf", options);
}
}
}
```
### See Also
* class [PdfBookmarkEntry](../../../aspose.cells.rendering/pdfbookmarkentry/)
* class [PdfSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
