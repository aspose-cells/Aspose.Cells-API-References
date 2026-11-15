---
title: Aspose::Cells::Rendering::WorkbookPrintingPreview::GetEvaluatedPageCount method
linktitle: GetEvaluatedPageCount
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Rendering::WorkbookPrintingPreview::GetEvaluatedPageCount method. Evaluate the total page count of this workbook in C++.'
type: docs
weight: 600
url: /ru/cpp/aspose.cells.rendering/workbookprintingpreview/getevaluatedpagecount/
---
## WorkbookPrintingPreview::GetEvaluatedPageCount method


Evaluate the total page count of this workbook.

```cpp
int32_t Aspose::Cells::Rendering::WorkbookPrintingPreview::GetEvaluatedPageCount()
```


## Examples


```cpp
Aspose::Cells::Startup();
//Следующий код показывает самый быстрый способ получить количество страниц книги.
Workbook workbook(u"Book1.xlsx");

WorkbookPrintingPreview workbookPrintingPreview(workbook, ImageOrPrintOptions());

//самый быстрый способ получить количество страниц, особенно когда в книге огромные данные.
int pageCount = workbookPrintingPreview.GetEvaluatedPageCount();

Aspose::Cells::Cleanup();
```

## See Also

* Class [Vector](../../../aspose.cells/vector/)
* Class [WorkbookPrintingPreview](../)
* Namespace [Aspose::Cells::Rendering](../../)
* Library [Aspose.Cells for C++](../../../)
