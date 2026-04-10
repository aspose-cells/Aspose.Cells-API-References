---
title: Aspose::Cells::Rendering::SheetPrintingPreview::GetEvaluatedPageCount method
linktitle: GetEvaluatedPageCount
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Rendering::SheetPrintingPreview::GetEvaluatedPageCount method. Evaluate the total page count of this worksheet in C++.'
type: docs
weight: 600
url: /es/cpp/aspose.cells.rendering/sheetprintingpreview/getevaluatedpagecount/
---
## SheetPrintingPreview::GetEvaluatedPageCount method


Evaluate the total page count of this worksheet.

```cpp
int32_t Aspose::Cells::Rendering::SheetPrintingPreview::GetEvaluatedPageCount()
```


## Examples


```cpp
Aspose::Cells::Startup();
//El siguiente código muestra la forma más rápida de obtener el recuento de páginas de una hoja de cálculo.
Workbook workbook(u"Book1.xlsx");

SheetPrintingPreview sheetPrintingPreview(workbook.GetWorksheets().Get(0), ImageOrPrintOptions());

//la forma más rápida de obtener el recuento de páginas, especialmente cuando hay datos masivos en la hoja de cálculo.
int pageCount = sheetPrintingPreview.GetEvaluatedPageCount();

Aspose::Cells::Cleanup();
```

## See Also

* Class [Vector](../../../aspose.cells/vector/)
* Class [SheetPrintingPreview](../)
* Namespace [Aspose::Cells::Rendering](../../)
* Library [Aspose.Cells for C++](../../../)
