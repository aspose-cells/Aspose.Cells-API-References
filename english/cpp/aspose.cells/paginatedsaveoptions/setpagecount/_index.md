﻿---
title: Aspose::Cells::PaginatedSaveOptions::SetPageCount method
linktitle: SetPageCount
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::PaginatedSaveOptions::SetPageCount method. Gets or sets the number of pages to save in C++.'
type: docs
weight: 2400
url: /cpp/aspose.cells/paginatedsaveoptions/setpagecount/
---
## PaginatedSaveOptions::SetPageCount method


Gets or sets the number of pages to save.

```cpp
void Aspose::Cells::PaginatedSaveOptions::SetPageCount(int32_t value)
```

## Remarks


Default is System.Int32.MaxValue which means all pages will be rendered.. 

## Examples


```cpp
Aspose::Cells::Startup();
//The following example shows how to render a range of pages (3 and 4) in a Microsoft Excel file to PDF.
 //Open an Excel file
Workbook wb(u"Book1.xlsx");

PdfSaveOptions options;

//Print only Page 3 and Page 4 in the output PDF
//Starting page index (0-based index)
if (options.GetPageIndex() != 3)
{
    options.SetPageIndex(3);
}
//Number of pages to be printed
if (options.GetPageCount() != 2)
{
    options.SetPageCount(2);
}

//Save the PDF file
wb.Save(u"output.pdf", options);
Aspose::Cells::Cleanup();
```

## See Also

* Class [Vector](../../vector/)
* Class [PaginatedSaveOptions](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
