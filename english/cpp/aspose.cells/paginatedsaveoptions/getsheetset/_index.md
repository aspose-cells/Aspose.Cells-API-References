---
title: Aspose::Cells::PaginatedSaveOptions::GetSheetSet method
linktitle: GetSheetSet
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::PaginatedSaveOptions::GetSheetSet method. Gets or sets the sheets to render. Default is all visible sheets in the workbook: Aspose.Cells.Rendering.SheetSet.Visible in C++.'
type: docs
weight: 3600
url: /cpp/aspose.cells/paginatedsaveoptions/getsheetset/
---
## PaginatedSaveOptions::GetSheetSet method


Gets or sets the sheets to render. Default is all visible sheets in the workbook: Aspose.Cells.Rendering.SheetSet.Visible.

```cpp
SheetSet Aspose::Cells::PaginatedSaveOptions::GetSheetSet()
```


## Examples


```cpp
Aspose::Cells::Startup();
//The following code only renders active sheet to pdf.
Workbook workbook(u"Book1.xlsx");

int activeSheetIndex = workbook.GetWorksheets().GetActiveSheetIndex();

PdfSaveOptions pdfSaveOptions;
//set active sheet index to sheet set.
SheetSet sheetSet = pdfSaveOptions.GetSheetSet();
if(!sheetSet.IsNull())
{
    //do what you want
}
workbook.Save(u"output.pdf", pdfSaveOptions);
Aspose::Cells::Cleanup();
```

## See Also

* Class [SheetSet](../../../aspose.cells.rendering/sheetset/)
* Class [PaginatedSaveOptions](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
