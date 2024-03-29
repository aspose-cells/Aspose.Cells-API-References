---
title: PaginatedSaveOptions.PageIndex
second_title: Aspose.Cells for .NET API Reference
description: PaginatedSaveOptions property. Gets or sets the 0based index of the first page to save
type: docs
url: /net/aspose.cells/paginatedsaveoptions/pageindex/
---
## PaginatedSaveOptions.PageIndex property

Gets or sets the 0-based index of the first page to save.

```csharp
public int PageIndex { get; set; }
```

### Remarks

Default is 0.

### Examples

The following example shows how to render a range of pages (3 and 4) in a Microsoft Excel file to PDF.

```csharp
//Open an Excel file
Workbook wb = new Workbook("Book1.xlsx");

PdfSaveOptions options = new PdfSaveOptions();

//Print only Page 3 and Page 4 in the output PDF
//Starting page index (0-based index)
options.PageIndex = 3;
//Number of pages to be printed
options.PageCount = 2;

//Save the PDF file
wb.Save("output.pdf", options);
```

### See Also

* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


