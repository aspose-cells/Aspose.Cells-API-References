---
title: PdfSaveOptions.Bookmark
second_title: Aspose.Cells for .NET API Reference
description: PdfSaveOptions property. Gets and sets the PdfBookmarkEntry object
type: docs
url: /net/aspose.cells/pdfsaveoptions/bookmark/
---
## PdfSaveOptions.Bookmark property

Gets and sets the [`PdfBookmarkEntry`](../../../aspose.cells.rendering/pdfbookmarkentry/) object.

```csharp
public PdfBookmarkEntry Bookmark { get; set; }
```

### Examples

```csharp
// Called: pdfSaveOptions.Bookmark = entry;
[Test, Description(&quot;PdfSaveOptions.Bookmark property need be checked by Manual&quot;)]
        public void Property_Bookmark()
        {
            string FileName = Constants.sourcePath + &quot;TestWorkbook\\Book2.xls&quot;;
            Workbook workbook = new Workbook(FileName);
            Cells cells = workbook.Worksheets[0].Cells;
            cells[0, 0].PutValue(&quot;page1&quot;);
            PdfBookmarkEntry entry = new PdfBookmarkEntry();
            entry.Text = &quot;section1&quot;;
            entry.Destination = cells[0, 0];
            entry.IsOpen = true;
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            pdfSaveOptions.Bookmark = entry;
            workbook.Save(Constants.checkPath + &quot;PdfSaveOptions_Bookmark_001.pdf&quot;, pdfSaveOptions);
        }
```

### See Also

* class [PdfBookmarkEntry](../../../aspose.cells.rendering/pdfbookmarkentry/)
* class [PdfSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


