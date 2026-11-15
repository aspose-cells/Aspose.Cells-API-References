---
title: Aspose::Cells::Rendering::SheetPrintingPreview::GetEvaluatedPageCount method
linktitle: GetEvaluatedPageCount
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Rendering::SheetPrintingPreview::GetEvaluatedPageCount method. Evaluate the total page count of this worksheet in C++.'
type: docs
weight: 600
url: /sv/cpp/aspose.cells.rendering/sheetprintingpreview/getevaluatedpagecount/
---
## SheetPrintingPreview::GetEvaluatedPageCount method


Evaluate the total page count of this worksheet.

```cpp
int32_t Aspose::Cells::Rendering::SheetPrintingPreview::GetEvaluatedPageCount()
```


## Examples


```cpp
Aspose::Cells::Startup();
//Följande kod visar det snabbaste sättet att få sidantalet för ett kalkylblad.
Workbook workbook(u"Book1.xlsx");

SheetPrintingPreview sheetPrintingPreview(workbook.GetWorksheets().Get(0), ImageOrPrintOptions());

//snabbaste sättet att få sidantalet, särskilt när det finns massiva data i kalkylbladet.
int pageCount = sheetPrintingPreview.GetEvaluatedPageCount();

Aspose::Cells::Cleanup();
```

## See Also

* Class [Vector](../../../aspose.cells/vector/)
* Class [SheetPrintingPreview](../)
* Namespace [Aspose::Cells::Rendering](../../)
* Library [Aspose.Cells for C++](../../../)
