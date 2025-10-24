##PdfBookmarkEntry.SubEntry
PdfBookmarkEntry property. SubEntry of a bookmark
## PdfBookmarkEntry.SubEntry property
SubEntry of a bookmark.
```csharp
public ArrayList SubEntry { get; set; }
```
### Examples
```csharp
using System;
using System.Collections;
using Aspose.Cells;
using Aspose.Cells.Rendering;
namespace AsposeCellsExamples
{
public class PdfBookmarkEntryPropertySubEntryDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
workbook.Worksheets.Add("Sheet2");
workbook.Worksheets.Add("Sheet3");
// Create root bookmark entry
PdfBookmarkEntry root = new PdfBookmarkEntry
{
Text = "Main Bookmark",
Destination = workbook.Worksheets[0].Cells["A1"],
SubEntry = new ArrayList(),
IsOpen = true
};
// Create sub-bookmarks
PdfBookmarkEntry sub1 = new PdfBookmarkEntry
{
Text = "First Section",
Destination = workbook.Worksheets[1].Cells["A1"]
};
PdfBookmarkEntry sub2 = new PdfBookmarkEntry
{
Text = "Second Section",
Destination = workbook.Worksheets[2].Cells["A1"],
SubEntry = new ArrayList()
};
// Add nested sub-bookmark
PdfBookmarkEntry subSub = new PdfBookmarkEntry
{
Text = "Sub-Section",
Destination = workbook.Worksheets[2].Cells["B1"]
};
sub2.SubEntry.Add(subSub);
// Add sub-bookmarks to root
root.SubEntry.Add(sub1);
root.SubEntry.Add(sub2);
// Save with bookmarks
PdfSaveOptions options = new PdfSaveOptions
{
Bookmark = root
};
workbook.Save("output_with_bookmarks.pdf", options);
}
}
}
```
### See Also
* class [PdfBookmarkEntry](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)
