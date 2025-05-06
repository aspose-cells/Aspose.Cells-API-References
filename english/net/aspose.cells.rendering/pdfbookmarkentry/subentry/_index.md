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
// Called: pbeRoot.SubEntry = subEntryList;
[Test]
        public void Property_SubEntry()
        {
            Workbook workbook = new Workbook();

            // Get the worksheets in the workbook.
            WorksheetCollection worksheets = workbook.Worksheets;

            // Add a sheet to the workbook.
            worksheets.Add(&quot;1&quot;);

            // Add 2nd sheet to the workbook.
            worksheets.Add(&quot;2&quot;);

            // Add the third sheet.
            worksheets.Add(&quot;3&quot;);

            // Get cells in different worksheets.
            Cell cellInPage1 = worksheets[0].Cells[&quot;A1&quot;];
            Cell cellInPage2 = worksheets[1].Cells[&quot;A1&quot;]; ;
            Cell cellInPage3 = worksheets[2].Cells[&quot;A1&quot;]; ;

            // Add a value to the A1 cell in the first sheet.
            cellInPage1.Value = &quot;a&quot;;

            // Add a value to the A1 cell in the second sheet.
            cellInPage2.Value = &quot;b&quot;;

            // Add a value to the A1 cell in the third sheet.
            cellInPage3.Value = &quot;c&quot;;

            // Create the PdfBookmark entry object.
            PdfBookmarkEntry pbeRoot = new PdfBookmarkEntry();

            // Set its text.
            //pbeRoot.Text = &quot;root&quot;;
            pbeRoot.Text = &quot;&quot;;

            // Set its destination source page.
            pbeRoot.Destination = cellInPage1;

            // Set the bookmark collapsed.
            pbeRoot.IsOpen = false;

            // Add a new PdfBookmark entry object.
            PdfBookmarkEntry subPbe1 = new PdfBookmarkEntry();

            // Set its text.
            subPbe1.Text = &quot;1&quot;;

            // Set its destination source page.
            subPbe1.Destination = cellInPage2;

            // Add another PdfBookmark entry object.
            PdfBookmarkEntry subPbe2 = new PdfBookmarkEntry();

            // Set its text.
            subPbe2.Text = &quot;2&quot;;

            // Set its destination source page.
            subPbe2.Destination = cellInPage3;

            // Create an array list.
            ArrayList subEntryList = new ArrayList();

            // Add the entry objects to it.
            subEntryList.Add(subPbe1);
            subEntryList.Add(subPbe2);
            pbeRoot.SubEntry = subEntryList;

            // Set the PDF bookmarks.
            PdfSaveOptions options = new PdfSaveOptions();
            options.Bookmark = pbeRoot;

            options.PageIndex = 2;
            options.PageCount = 1;

            // Save the PDF file.
            workbook.Save(new MemoryStream(), options);
        }
```

### See Also

* class [PdfBookmarkEntry](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


