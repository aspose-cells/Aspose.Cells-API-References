---
title: Aspose::Cells::Rendering::WorkbookPrintingPreview::GetEvaluatedPageCount method
linktitle: GetEvaluatedPageCount
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Rendering::WorkbookPrintingPreview::GetEvaluatedPageCount method. Evaluate the total page count of this workbook in C++.'
type: docs
weight: 600
url: /tr/cpp/aspose.cells.rendering/workbookprintingpreview/getevaluatedpagecount/
---
## WorkbookPrintingPreview::GetEvaluatedPageCount method


Evaluate the total page count of this workbook.

```cpp
int32_t Aspose::Cells::Rendering::WorkbookPrintingPreview::GetEvaluatedPageCount()
```


## Examples


```cpp
Aspose::Cells::Startup();
//Aşağıdaki kod, bir çalışma kitabının sayfa sayısını almanın en hızlı yolunu gösterir.
Workbook workbook(u"Book1.xlsx");

WorkbookPrintingPreview workbookPrintingPreview(workbook, ImageOrPrintOptions());

//Çalışma kitabında büyük veri olduğunda sayfa sayısını almanın en hızlı yolu.
int pageCount = workbookPrintingPreview.GetEvaluatedPageCount();

Aspose::Cells::Cleanup();
```

## See Also

* Class [Vector](../../../aspose.cells/vector/)
* Class [WorkbookPrintingPreview](../)
* Namespace [Aspose::Cells::Rendering](../../)
* Library [Aspose.Cells for C++](../../../)
