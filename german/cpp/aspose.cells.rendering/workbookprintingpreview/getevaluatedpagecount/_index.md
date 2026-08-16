---
title: Aspose::Cells::Rendering::WorkbookPrintingPreview::GetEvaluatedPageCount method
linktitle: GetEvaluatedPageCount
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Rendering::WorkbookPrintingPreview::GetEvaluatedPageCount method. Evaluate the total page count of this workbook in C++.'
type: docs
weight: 600
url: /de/cpp/aspose.cells.rendering/workbookprintingpreview/getevaluatedpagecount/
---
## WorkbookPrintingPreview::GetEvaluatedPageCount method


Evaluate the total page count of this workbook.

```cpp
int32_t Aspose::Cells::Rendering::WorkbookPrintingPreview::GetEvaluatedPageCount()
```


## Examples


```cpp
Aspose::Cells::Startup();
//Der folgende Code zeigt den schnellsten Weg, die Seitenzahl einer Arbeitsmappe zu ermitteln.
Workbook workbook(u"Book1.xlsx");

WorkbookPrintingPreview workbookPrintingPreview(workbook, ImageOrPrintOptions());

//Schnellster Weg, die Seitenzahl zu ermitteln, insbesondere wenn massive Daten in der Arbeitsmappe vorhanden sind.
int pageCount = workbookPrintingPreview.GetEvaluatedPageCount();

Aspose::Cells::Cleanup();
```

## See Also

* Class [Vector](../../../aspose.cells/vector/)
* Class [WorkbookPrintingPreview](../)
* Namespace [Aspose::Cells::Rendering](../../)
* Library [Aspose.Cells for C++](../../../)
