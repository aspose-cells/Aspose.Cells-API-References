---
title: Aspose::Cells::Rendering::WorkbookPrintingPreview::GetEvaluatedPageCount method
linktitle: GetEvaluatedPageCount
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Rendering::WorkbookPrintingPreview::GetEvaluatedPageCount method. Evaluate the total page count of this workbook in C++.'
type: docs
weight: 600
url: /ar/cpp/aspose.cells.rendering/workbookprintingpreview/getevaluatedpagecount/
---
## WorkbookPrintingPreview::GetEvaluatedPageCount method


Evaluate the total page count of this workbook.

```cpp
int32_t Aspose::Cells::Rendering::WorkbookPrintingPreview::GetEvaluatedPageCount()
```


## Examples


```cpp
Aspose::Cells::Startup();
//الكود التالي يوضح أسرع طريقة للحصول على عدد الصفحات في دفتر العمل.
Workbook workbook(u"Book1.xlsx");

WorkbookPrintingPreview workbookPrintingPreview(workbook, ImageOrPrintOptions());

//أسرع طريقة للحصول على عدد الصفحات خاصةً عندما تكون هناك بيانات ضخمة في دفتر العمل.
int pageCount = workbookPrintingPreview.GetEvaluatedPageCount();

Aspose::Cells::Cleanup();
```

## See Also

* Class [Vector](../../../aspose.cells/vector/)
* Class [WorkbookPrintingPreview](../)
* Namespace [Aspose::Cells::Rendering](../../)
* Library [Aspose.Cells for C++](../../../)
