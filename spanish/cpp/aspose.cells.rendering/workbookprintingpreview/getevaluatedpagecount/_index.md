---
title: Aspose::Cells::Rendering::WorkbookPrintingPreview::GetEvaluatedPageCount method
linktitle: GetEvaluatedPageCount
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Rendering::WorkbookPrintingPreview::GetEvaluatedPageCount method. Evaluate the total page count of this workbook in C++.'
type: docs
weight: 600
url: /es/cpp/aspose.cells.rendering/workbookprintingpreview/getevaluatedpagecount/
---
## WorkbookPrintingPreview::GetEvaluatedPageCount method


Evaluate the total page count of this workbook.

```cpp
int32_t Aspose::Cells::Rendering::WorkbookPrintingPreview::GetEvaluatedPageCount()
```


## Examples


```cpp
Aspose::Cells::Startup();
//El siguiente código muestra la forma más rápida de obtener el recuento de páginas de un libro de trabajo.
Workbook workbook(u"Book1.xlsx");

WorkbookPrintingPreview workbookPrintingPreview(workbook, ImageOrPrintOptions());

//la forma más rápida de obtener el recuento de páginas, especialmente cuando hay datos masivos en el libro de trabajo.
int pageCount = workbookPrintingPreview.GetEvaluatedPageCount();

Aspose::Cells::Cleanup();
```

## See Also

* Class [Vector](../../../aspose.cells/vector/)
* Class [WorkbookPrintingPreview](../)
* Namespace [Aspose::Cells::Rendering](../../)
* Library [Aspose.Cells for C++](../../../)
