---
title: Class PdfBookmarkEntry
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.Rendering.PdfBookmarkEntry class. PdfBookmarkEntry is an entry in pdf bookmark. if Text property of current instance is null or  current instance will be hidden and children will be inserted on current level
type: docs
url: /net/aspose.cells.rendering/pdfbookmarkentry/
---
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
[C#]    
orkbook workbook = new Workbook();
orkbook.Worksheets.Add();
orkbook.Worksheets.Add();
ell cellInPage1 = workbook.Worksheets[0].Cells["A1"];
ell cellInPage2 = workbook.Worksheets[1].Cells["A1"];
ell cellInPage3 = workbook.Worksheets[2].Cells["A1"];
ellInPage1.PutValue("page1");
ellInPage2.PutValue("page2");
ellInPage3.PutValue("page3");

dfBookmarkEntry pbeRoot = new PdfBookmarkEntry();
beRoot.Text = "root";  // if pbeRoot.Text = null, all children of pbeRoot will be inserted on the top level in the bookmark.
beRoot.Destination = cellInPage1;
beRoot.SubEntry = new ArrayList();
beRoot.IsOpen = false;

dfBookmarkEntry subPbe1 = new PdfBookmarkEntry();
ubPbe1.Text = "section1";
ubPbe1.Destination = cellInPage2;

dfBookmarkEntry subPbe2 = new PdfBookmarkEntry();
ubPbe2.Text = "section2";
ubPbe2.Destination = cellInPage3;

beRoot.SubEntry.Add(subPbe1);
beRoot.SubEntry.Add(subPbe2);

dfSaveOptions saveOptions = new PdfSaveOptions();
aveOptions.Bookmark = pbeRoot;
orkbook.Save("output_bookmark.pdf", saveOptions);

[VB]    
im workbook As Workbook = New Workbook
orkbook.Worksheets.Add("sheet2")
orkbook.Worksheets.Add("sheet3")

im cells As Cells = workbook.Worksheets(0).Cells
im cellInPage1 As Cell = cells("A1")
ellInPage1.PutValue("Page1")

ells = workbook.Worksheets(1).Cells
im cellInPage2 As Cell = cells("A1")
ellInPage2.PutValue("Page2")

ells = workbook.Worksheets(2).Cells
im cellInPage3 As Cell = cells("A1")
ellInPage3.PutValue("Page3")

im pbeRoot As PdfBookmarkEntry = New PdfBookmarkEntry()
beRoot.Text = "root"
beRoot.Destination = cellInPage1
beRoot.SubEntry = New ArrayList
beRoot.IsOpen = False

im subPbe1 As PdfBookmarkEntry = New PdfBookmarkEntry()
ubPbe1.Text = "section1"
ubPbe1.Destination = cellInPage2

im subPbe2 As PdfBookmarkEntry = New PdfBookmarkEntry()
ubPbe2.Text = "section2"
ubPbe2.Destination = cellInPage3

beRoot.SubEntry.Add(subPbe1)
beRoot.SubEntry.Add(subPbe2)

im saveOptions As PdfSaveOptions = New PdfSaveOptions()
aveOptions.Bookmark = pbeRoot
orkbook.Save("output_bookmark.pdf", saveOptions)
```

### See Also

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


