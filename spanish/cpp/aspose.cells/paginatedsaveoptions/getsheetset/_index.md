---
title: Aspose::Cells::PaginatedSaveOptions::GetSheetSet method
linktitle: GetSheetSet
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::PaginatedSaveOptions::GetSheetSet method. Gets or sets the sheets to render. Default is all visible sheets in the workbook: Aspose.Cells.Rendering.SheetSet.Visible in C++.'
type: docs
weight: 3600
url: /es/cpp/aspose.cells/paginatedsaveoptions/getsheetset/
---
## PaginatedSaveOptions::GetSheetSet method


Gets or sets the sheets to render. Default is all visible sheets in the workbook: Aspose.Cells.Rendering.SheetSet.Visible.

```cpp
SheetSet Aspose::Cells::PaginatedSaveOptions::GetSheetSet()
```


## Examples


```cpp
Aspose::Cells::Startup();
//El siguiente código solo renderiza la hoja activa a PDF.
Workbook workbook(u"Book1.xlsx");

int activeSheetIndex = workbook.GetWorksheets().GetActiveSheetIndex();

PdfSaveOptions pdfSaveOptions;
//establecer el índice de la hoja activa al conjunto de hojas.
SheetSet sheetSet = pdfSaveOptions.GetSheetSet();
if(!sheetSet.IsNull())
{
    //haz lo que quieras
}
workbook.Save(u"output.pdf", pdfSaveOptions);
Aspose::Cells::Cleanup();
```

## See Also

* Class [SheetSet](../../../aspose.cells.rendering/sheetset/)
* Class [PaginatedSaveOptions](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
