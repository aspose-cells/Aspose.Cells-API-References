##Class PdfBookmarkEntry
Aspose.Cells.Rendering.PdfBookmarkEntry class. PdfBookmarkEntry is an entry in pdf bookmark. if Text property of current instance is null or  current instance will be hidden and children will be inserted on current level
## PdfBookmarkEntry class
PdfBookmarkEntry is an entry in pdf bookmark. if Text property of current instance is null or "", current instance will be hidden and children will be inserted on current level.
```csharp
public class PdfBookmarkEntry
```
## Constructors
| Name | Description |
| --- | --- |
| [PdfBookmarkEntry](pdfbookmarkentry/)() | The default constructor. |
## Properties
| Name | Description |
| --- | --- |
| [Destination](../../aspose.cells.rendering/pdfbookmarkentry/destination/) { get; set; } | The cell to which the bookmark link. |
| [DestinationName](../../aspose.cells.rendering/pdfbookmarkentry/destinationname/) { get; set; } | Gets or sets name of destination. |
| [IsCollapse](../../aspose.cells.rendering/pdfbookmarkentry/iscollapse/) { get; set; } | When this property is true, the bookmarkentry will collapse, otherwise it will expand. |
| [IsOpen](../../aspose.cells.rendering/pdfbookmarkentry/isopen/) { get; set; } | When this property is true, the bookmarkentry will expand, otherwise it will collapse. |
| [SubEntry](../../aspose.cells.rendering/pdfbookmarkentry/subentry/) { get; set; } | SubEntry of a bookmark. |
| [Text](../../aspose.cells.rendering/pdfbookmarkentry/text/) { get; set; } | Title of a bookmark. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Rendering;
using System;
using System.Collections;
public class PdfBookmarkEntryDemo
{
public static void PdfBookmarkEntryExample()
{
// Create a new workbook and add worksheets
Workbook workbook = new Workbook();
workbook.Worksheets.Add();
workbook.Worksheets.Add();
// Get cells from each worksheet
Cell cellInPage1 = workbook.Worksheets[0].Cells["A1"];
Cell cellInPage2 = workbook.Worksheets[1].Cells["A1"];
Cell cellInPage3 = workbook.Worksheets[2].Cells["A1"];
// Put values in the cells
cellInPage1.PutValue("page1");
cellInPage2.PutValue("page2");
cellInPage3.PutValue("page3");
// Create the root PdfBookmarkEntry
PdfBookmarkEntry pbeRoot = new PdfBookmarkEntry
{
Text = "root",  // if pbeRoot.Text = null, all children of pbeRoot will be inserted on the top level in the bookmark.
Destination = cellInPage1,
SubEntry = new ArrayList(),
IsOpen = false
};
// Create sub PdfBookmarkEntries
PdfBookmarkEntry subPbe1 = new PdfBookmarkEntry
{
Text = "section1",
Destination = cellInPage2
};
PdfBookmarkEntry subPbe2 = new PdfBookmarkEntry
{
Text = "section2",
Destination = cellInPage3
};
// Add sub entries to the root entry
pbeRoot.SubEntry.Add(subPbe1);
pbeRoot.SubEntry.Add(subPbe2);
// Create PdfSaveOptions and set the bookmark
PdfSaveOptions saveOptions = new PdfSaveOptions
{
Bookmark = pbeRoot
};
// Save the workbook as a PDF with bookmarks
workbook.Save("output_bookmark.pdf", saveOptions);
}
}
}
```
### See Also
* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)
