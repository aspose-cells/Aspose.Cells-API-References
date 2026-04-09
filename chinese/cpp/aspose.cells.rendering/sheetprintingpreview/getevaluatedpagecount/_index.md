---
title: Aspose::Cells::Rendering::SheetPrintingPreview::GetEvaluatedPageCount method
linktitle: GetEvaluatedPageCount
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Rendering::SheetPrintingPreview::GetEvaluatedPageCount method. Evaluate the total page count of this worksheet in C++.'
type: docs
weight: 600
url: /zh/cpp/aspose.cells.rendering/sheetprintingpreview/getevaluatedpagecount/
---
## SheetPrintingPreview::GetEvaluatedPageCount method


Evaluate the total page count of this worksheet.

```cpp
int32_t Aspose::Cells::Rendering::SheetPrintingPreview::GetEvaluatedPageCount()
```


## Examples


```cpp
Aspose::Cells::Startup();
//以下代码展示了获取工作表页数的最快方法。
Workbook workbook(u"Book1.xlsx");

SheetPrintingPreview sheetPrintingPreview(workbook.GetWorksheets().Get(0), ImageOrPrintOptions());

//在工作表中有大量数据时，获取页数的最快方法。
int pageCount = sheetPrintingPreview.GetEvaluatedPageCount();

Aspose::Cells::Cleanup();
```

## See Also

* Class [Vector](../../../aspose.cells/vector/)
* Class [SheetPrintingPreview](../)
* Namespace [Aspose::Cells::Rendering](../../)
* Library [Aspose.Cells for C++](../../../)
