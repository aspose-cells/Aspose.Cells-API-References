---
title: PdfBookmarkEntry.IsOpen
second_title: Aspose.Cells for .NET API Reference
description: PdfBookmarkEntry property. When this property is true the bookmarkentry will expand otherwise it will collapse
type: docs
url: /net/aspose.cells.rendering/pdfbookmarkentry/isopen/
---
## PdfBookmarkEntry.IsOpen property

When this property is true, the bookmarkentry will expand, otherwise it will collapse.

```csharp
public bool IsOpen { get; set; }
```

### Examples

```csharp
// Called: pbeRoot.IsOpen = false;
[Test]
        public void Property_IsOpen()
        {
            Workbook workbook = new Workbook();

            // Get the worksheets in the workbook.
            WorksheetCollection worksheets = workbook.Worksheets;

            // Add a sheet to the workbook.
            worksheets.Add("1");

            // Add 2nd sheet to the workbook.
            worksheets.Add("2");

            // Add the third sheet.
            worksheets.Add("3");

            // Get cells in different worksheets.
            Cell cellInPage1 = worksheets[0].Cells["A1"];
            Cell cellInPage2 = worksheets[1].Cells["A1"]; ;
            Cell cellInPage3 = worksheets[2].Cells["A1"]; ;

            // Add a value to the A1 cell in the first sheet.
            cellInPage1.Value = "a";

            // Add a value to the A1 cell in the second sheet.
            cellInPage2.Value = "b";

            // Add a value to the A1 cell in the third sheet.
            cellInPage3.Value = "c";

            // Create the PdfBookmark entry object.
            PdfBookmarkEntry pbeRoot = new PdfBookmarkEntry();

            // Set its text.
            //pbeRoot.Text = "root";
            pbeRoot.Text = "";

            // Set its destination source page.
            pbeRoot.Destination = cellInPage1;

            // Set the bookmark collapsed.
            pbeRoot.IsOpen = false;

            // Add a new PdfBookmark entry object.
            PdfBookmarkEntry subPbe1 = new PdfBookmarkEntry();

            // Set its text.
            subPbe1.Text = "1";

            // Set its destination source page.
            subPbe1.Destination = cellInPage2;

            // Add another PdfBookmark entry object.
            PdfBookmarkEntry subPbe2 = new PdfBookmarkEntry();

            // Set its text.
            subPbe2.Text = "2";

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


