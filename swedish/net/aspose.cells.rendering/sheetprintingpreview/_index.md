---
title: "Klass SheetPrintingPreview"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Rendering.SheetPrintingPreview-klass. Utskriftsförhandsgranskning av kalkylblad"
type: docs
url: /sv/net/aspose.cells.rendering/sheetprintingpreview/
---
## SheetPrintingPreview class

Utskriftsförhandsgranskning för arbetsblad.

```csharp
public class SheetPrintingPreview
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [SheetPrintingPreview](sheetprintingpreview/)(Worksheet, ImageOrPrintOptions) | Konstruktionen av SheetPrintingPreview |

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [EvaluatedPageCount](../../aspose.cells.rendering/sheetprintingpreview/evaluatedpagecount/) { get; } | Utvärdera det totala sidantalet i detta kalkylblad |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class SheetPrintingPreviewDemo
    {
        public static void SheetPrintingPreviewExample()
        {
            // Läs in en befintlig arbetsbok
            Workbook workbook = new Workbook("SheetPrintingPreviewDemo_original.xlsx");

            // Hämta det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa en instans av ImageOrPrintOptions
            ImageOrPrintOptions options = new ImageOrPrintOptions();

            // Skapa en instans av SheetPrintingPreview
            SheetPrintingPreview sheetPrintingPreview = new SheetPrintingPreview(worksheet, options);

            // Utvärdera och skriv ut det totala sidantalet för kalkylbladet
            Console.WriteLine("Total Page Count: " + sheetPrintingPreview.EvaluatedPageCount);
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


