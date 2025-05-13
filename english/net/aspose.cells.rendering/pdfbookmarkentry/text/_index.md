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
// Called: entry.Text = "section1";
[Test, Description("PdfSaveOptions.Bookmark property need be checked by Manual")]
        public void PdfBookmarkEntry_Property_Text()
        {
            string FileName = Constants.sourcePath + "TestWorkbook\\Book2.xls";
            Workbook workbook = new Workbook(FileName);
            Cells cells = workbook.Worksheets[0].Cells;
            cells[0, 0].PutValue("page1");
            PdfBookmarkEntry entry = new PdfBookmarkEntry();
            entry.Text = "section1";
            entry.Destination = cells[0, 0];
            entry.IsOpen = true;
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            pdfSaveOptions.Bookmark = entry;
            workbook.Save(Constants.checkPath + "example.pdf", pdfSaveOptions);
        }
```

### See Also

* class [PdfBookmarkEntry](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


