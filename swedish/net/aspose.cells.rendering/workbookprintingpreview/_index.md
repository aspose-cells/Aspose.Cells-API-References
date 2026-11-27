---
title: "Klass WorkbookPrintingPreview"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Rendering.WorkbookPrintingPreview-klass. Förhandsgranskning av arbetsboksutskrift"
type: docs
url: /sv/net/aspose.cells.rendering/workbookprintingpreview/
---
## WorkbookPrintingPreview class

Utskriftsförhandsgranskning för arbetsbok.

```csharp
public class WorkbookPrintingPreview
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [WorkbookPrintingPreview](workbookprintingpreview/)(Workbook, ImageOrPrintOptions) | Konstruktionen av WorkbookPrintingPreview |

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [EvaluatedPageCount](../../aspose.cells.rendering/workbookprintingpreview/evaluatedpagecount/) { get; } | Utvärdera det totala sidantalet i den här arbetsboken |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class WorkbookPrintingPreviewDemo
    {
        public static void WorkbookPrintingPreviewExample()
        {
            // Läs in en befintlig arbetsbok
            Workbook workbook = new Workbook("WorkbookPrintingPreviewExample_original.xlsx");

            // Skapa en instans av ImageOrPrintOptions
            ImageOrPrintOptions options = new ImageOrPrintOptions();

            // Skapa en instans av WorkbookPrintingPreview
            WorkbookPrintingPreview workbookPrintingPreview = new WorkbookPrintingPreview(workbook, options);

            // Utvärdera det totala sidantalet i arbetsboken
            int pageCount = workbookPrintingPreview.EvaluatedPageCount;

            // Skriv ut det utvärderade sidantalet
            Console.WriteLine("Total Page Count: " + pageCount);
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


