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
// Called: entry.IsOpen = false;
[Test, Description(&quot;PdfSaveOptions.Bookmark property need be checked by Manual&quot;)]
        public void Property_IsOpen()
        {
            string FileName = Constants.sourcePath + &quot;TestWorkbook\\Book2.xls&quot;;
            Workbook workbook = new Workbook(FileName);
            Cells cells = workbook.Worksheets[0].Cells;
            cells[0, 0].PutValue(&quot;page1&quot;);
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            PdfBookmarkEntry entry = new PdfBookmarkEntry();
            entry.Text = &quot;section1&quot;;
            entry.Destination = cells[0, 0];
            entry.IsOpen = false;
            pdfSaveOptions.Bookmark = entry;
            workbook.Save(Constants.checkPath + &quot;PdfSaveOptions_Bookmark_002.pdf&quot;, pdfSaveOptions);
        }
```

### See Also

* class [PdfBookmarkEntry](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


