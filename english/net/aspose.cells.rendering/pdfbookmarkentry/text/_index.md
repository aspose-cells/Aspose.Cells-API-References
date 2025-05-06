---
title: PdfBookmarkEntry.Text
second_title: Aspose.Cells for .NET API Reference
description: PdfBookmarkEntry property. Title of a bookmark
type: docs
url: /net/aspose.cells.rendering/pdfbookmarkentry/text/
---
## PdfBookmarkEntry.Text property

Title of a bookmark.

```csharp
public string Text { get; set; }
```

### Examples

```csharp
// Called: Text = &amp;quot;root&amp;quot;,  // if pbeRoot.Text = null, all children of pbeRoot will be inserted on the top level in the bookmark.
public static void Property_Text()
        {
            // Create a new workbook and add worksheets
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add();
            workbook.Worksheets.Add();

            // Get cells from each worksheet
            Cell cellInPage1 = workbook.Worksheets[0].Cells[&quot;A1&quot;];
            Cell cellInPage2 = workbook.Worksheets[1].Cells[&quot;A1&quot;];
            Cell cellInPage3 = workbook.Worksheets[2].Cells[&quot;A1&quot;];

            // Put values in the cells
            cellInPage1.PutValue(&quot;page1&quot;);
            cellInPage2.PutValue(&quot;page2&quot;);
            cellInPage3.PutValue(&quot;page3&quot;);

            // Create the root PdfBookmarkEntry
            PdfBookmarkEntry pbeRoot = new PdfBookmarkEntry
            {
                Text = &quot;root&quot;,  // if pbeRoot.Text = null, all children of pbeRoot will be inserted on the top level in the bookmark.
                Destination = cellInPage1,
                SubEntry = new ArrayList(),
                IsOpen = false
            };

            // Create sub PdfBookmarkEntries
            PdfBookmarkEntry subPbe1 = new PdfBookmarkEntry
            {
                Text = &quot;section1&quot;,
                Destination = cellInPage2
            };

            PdfBookmarkEntry subPbe2 = new PdfBookmarkEntry
            {
                Text = &quot;section2&quot;,
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
            workbook.Save(&quot;output_bookmark.pdf&quot;, saveOptions);
        }
```

### See Also

* class [PdfBookmarkEntry](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


