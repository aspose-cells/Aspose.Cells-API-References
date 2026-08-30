---
title: Aspose::Cells::Rendering::SheetPrintingPreview::GetEvaluatedPageCount method
linktitle: GetEvaluatedPageCount
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Rendering::SheetPrintingPreview::GetEvaluatedPageCount method. Evaluate the total page count of this worksheet in C++.'
type: docs
weight: 600
url: /fr/cpp/aspose.cells.rendering/sheetprintingpreview/getevaluatedpagecount/
---
## SheetPrintingPreview::GetEvaluatedPageCount method


Evaluate the total page count of this worksheet.

```cpp
int32_t Aspose::Cells::Rendering::SheetPrintingPreview::GetEvaluatedPageCount()
```


## Examples


```cpp
Aspose::Cells::Startup();
//Le code suivant montre la façon la plus rapide d'obtenir le nombre de pages d'une feuille de calcul.
Workbook workbook(u"Book1.xlsx");

SheetPrintingPreview sheetPrintingPreview(workbook.GetWorksheets().Get(0), ImageOrPrintOptions());

//La façon la plus rapide d'obtenir le nombre de pages, surtout lorsqu'il y a des données massives dans la feuille de calcul.
int pageCount = sheetPrintingPreview.GetEvaluatedPageCount();

Aspose::Cells::Cleanup();
```

## See Also

* Class [Vector](../../../aspose.cells/vector/)
* Class [SheetPrintingPreview](../)
* Namespace [Aspose::Cells::Rendering](../../)
* Library [Aspose.Cells for C++](../../../)
