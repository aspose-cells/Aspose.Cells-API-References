---
title: EvaluatedPageCount
second_title: Aspose.Cells för .NET API-referens
description: Utvärdera det totala sidantalet för denna arbetsbok
type: docs
weight: 20
url: /sv/net/aspose.cells.rendering/workbookprintingpreview/evaluatedpagecount/
---
## WorkbookPrintingPreview.EvaluatedPageCount property

Utvärdera det totala sidantalet för denna arbetsbok

```csharp
public int EvaluatedPageCount { get; }
```

### Exempel

Följande kod visar det snabbaste sättet att få sidantal i en arbetsbok.

```csharp
Workbook workbook = new Workbook("Book1.xlsx");

WorkbookPrintingPreview workbookPrintingPreview = new WorkbookPrintingPreview(workbook, new ImageOrPrintOptions());

//snabbaste sättet att få sidräkning, särskilt när det finns massiva data i arbetsboken.
Console.WriteLine(workbookPrintingPreview.EvaluatedPageCount);
        
```

### Se även

* class [WorkbookPrintingPreview](../../workbookprintingpreview)
* namnutrymme [Aspose.Cells.Rendering](../../workbookprintingpreview)
* hopsättning [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
