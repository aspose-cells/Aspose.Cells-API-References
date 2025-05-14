---
title: PdfBookmarkEntry.Destination
second_title: Aspose.Cells for .NET API Reference
description: PdfBookmarkEntry property. The cell to which the bookmark link
type: docs
url: /net/aspose.cells.rendering/pdfbookmarkentry/destination/
---
## PdfBookmarkEntry.Destination property

The cell to which the bookmark link.

```csharp
public Cell Destination { get; set; }
```

### Examples

```csharp
// Called: entry.Destination = cells[0, 0];
[Test, Description("PdfSaveOptions.Bookmark property need be checked by Manual")]
        public void PdfBookmarkEntry_Property_Destination()
        {
            string FileName = Constants.sourcePath + "TestWorkbook\\Book2.xls";
            Workbook workbook = new Workbook(FileName);
            Cells cells = workbook.Worksheets[0].Cells;
            cells[0, 0].PutValue("page1");
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            PdfBookmarkEntry entry = new PdfBookmarkEntry();
            entry.Text = "section1";
            entry.Destination = cells[0, 0];
            entry.IsOpen = false;
            pdfSaveOptions.Bookmark = entry;
            workbook.Save(Constants.checkPath + "example.pdf", pdfSaveOptions);
        }
```

### See Also

* class [Cell](../../../aspose.cells/cell/)
* class [PdfBookmarkEntry](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


