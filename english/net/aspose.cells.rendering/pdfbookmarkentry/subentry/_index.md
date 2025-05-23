---
title: PdfBookmarkEntry.SubEntry
second_title: Aspose.Cells for .NET API Reference
description: PdfBookmarkEntry property. SubEntry of a bookmark
type: docs
url: /net/aspose.cells.rendering/pdfbookmarkentry/subentry/
---
## PdfBookmarkEntry.SubEntry property

SubEntry of a bookmark.

```csharp
public ArrayList SubEntry { get; set; }
```

### Examples

```csharp
// Called: SubEntry = new ArrayList(),
public static void PdfBookmarkEntry_Property_SubEntry()
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
```

### See Also

* class [PdfBookmarkEntry](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


