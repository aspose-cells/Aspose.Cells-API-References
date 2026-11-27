---
title: "SheetPrintingPreview.SheetPrintingPreview"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SheetPrintingPreview-konstruktor. Konstruktionen av SheetPrintingPreview"
type: docs
url: /sv/net/aspose.cells.rendering/sheetprintingpreview/sheetprintingpreview/
---
## SheetPrintingPreview constructor

Konstruktionen av SheetPrintingPreview

```csharp
public SheetPrintingPreview(Worksheet sheet, ImageOrPrintOptions options)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| blad | Arbetsblad | Ange vilket kalkylblad som ska skrivas ut. |
| alternativ | ImageOrPrintOptions | ImageOrPrintOptions innehåller vissa egenskaper för utdata |

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class SheetPrintingPreviewMethodctorWithWorksheetImageOrPrintOptionsDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok med exempeldata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata i arbetsbladet
            for (int i = 0; i < 10; i++)
            {
                for (int j = 0; j < 5; j++)
                {
                    worksheet.Cells[i, j].PutValue($"Data {i},{j}");
                }
            }

            // Skapa bild-/utskriftsalternativ
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.PrintingPage = PrintingPageType.Default;

            // Skapa förhandsgranskning av bladutskrift
            SheetPrintingPreview preview = new SheetPrintingPreview(worksheet, options);
            
            // Mata ut det beräknade sidantalet
            Console.WriteLine($"Evaluated page count: {preview.EvaluatedPageCount}");
        }
    }
}
```

### Se även

* class [Worksheet](../../../aspose.cells/worksheet/)
* class [ImageOrPrintOptions](../../imageorprintoptions/)
* class [SheetPrintingPreview](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


