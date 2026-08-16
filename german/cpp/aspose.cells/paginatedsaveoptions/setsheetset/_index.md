---
title: Aspose::Cells::PaginatedSaveOptions::SetSheetSet method
linktitle: SetSheetSet
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::PaginatedSaveOptions::SetSheetSet method. Gets or sets the sheets to render. Default is all visible sheets in the workbook: Aspose.Cells.Rendering.SheetSet.Visible in C++.'
type: docs
weight: 3700
url: /de/cpp/aspose.cells/paginatedsaveoptions/setsheetset/
---
## PaginatedSaveOptions::SetSheetSet method


Gets or sets the sheets to render. Default is all visible sheets in the workbook: Aspose.Cells.Rendering.SheetSet.Visible.

```cpp
void Aspose::Cells::PaginatedSaveOptions::SetSheetSet(const SheetSet &value)
```


## Examples


```cpp
Aspose::Cells::Startup();
//Der folgende Code rendert nur das aktive Blatt zu PDF.
Workbook workbook(u"Book1.xlsx");

int activeSheetIndex = workbook.GetWorksheets().GetActiveSheetIndex();

PdfSaveOptions pdfSaveOptions;
//Setze den Index des aktiven Blatts auf das Blatt-Set.
SheetSet sheetSet(Vector<int>{ activeSheetIndex });
pdfSaveOptions.SetSheetSet(sheetSet);
workbook.Save(u"output.pdf", pdfSaveOptions);
Aspose::Cells::Cleanup();
```

## See Also

* Class [Vector](../../vector/)
* Class [SheetSet](../../../aspose.cells.rendering/sheetset/)
* Class [PaginatedSaveOptions](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
