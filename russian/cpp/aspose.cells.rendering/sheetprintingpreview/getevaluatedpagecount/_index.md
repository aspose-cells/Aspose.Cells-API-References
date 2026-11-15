---
title: Aspose::Cells::Rendering::SheetPrintingPreview::GetEvaluatedPageCount method
linktitle: GetEvaluatedPageCount
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Rendering::SheetPrintingPreview::GetEvaluatedPageCount method. Evaluate the total page count of this worksheet in C++.'
type: docs
weight: 600
url: /ru/cpp/aspose.cells.rendering/sheetprintingpreview/getevaluatedpagecount/
---
## SheetPrintingPreview::GetEvaluatedPageCount method


Evaluate the total page count of this worksheet.

```cpp
int32_t Aspose::Cells::Rendering::SheetPrintingPreview::GetEvaluatedPageCount()
```


## Examples


```cpp
Aspose::Cells::Startup();
//Следующий код показывает самый быстрый способ получить количество страниц листа.
Workbook workbook(u"Book1.xlsx");

SheetPrintingPreview sheetPrintingPreview(workbook.GetWorksheets().Get(0), ImageOrPrintOptions());

//Самый быстрый способ получить количество страниц, особенно когда в листе огромные данные.
int pageCount = sheetPrintingPreview.GetEvaluatedPageCount();

Aspose::Cells::Cleanup();
```

## See Also

* Class [Vector](../../../aspose.cells/vector/)
* Class [SheetPrintingPreview](../)
* Namespace [Aspose::Cells::Rendering](../../)
* Library [Aspose.Cells for C++](../../../)
