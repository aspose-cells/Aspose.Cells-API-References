---
title: "Worksheet.GetPrintingPageBreaks"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Worksheet-metod. Hämtar automatiska sidbrytningar"
type: docs
url: /sv/net/aspose.cells/worksheet/getprintingpagebreaks/
---
## Worksheet.GetPrintingPageBreaks method

Hämtar automatiska sidbrytningar.

```csharp
public CellArea[] GetPrintingPageBreaks(ImageOrPrintOptions options)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| alternativ | ImageOrPrintOptions | Utskriftsalternativen |

### Returvärde

De automatiska sidbrytningsområdena.

### Anmärkningar

Varje cellområde representerar ett papper.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class WorksheetMethodGetPrintingPageBreaksWithImageOrPrintOptionsDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok med exempeldata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata för att skapa sidbrytningar
            for (int i = 0; i < 100; i++)
            {
                worksheet.Cells[$"A{i+1}"].PutValue($"Row {i+1}");
            }

            // Ställ in utskriftsområde och sidinställningar
            worksheet.PageSetup.PrintArea = "A1:A100";
            worksheet.PageSetup.FitToPagesTall = 1;
            worksheet.PageSetup.FitToPagesWide = 1;

            // Hämta sidbrytningar med ImageOrPrintOptions
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            CellArea[] pageBreaks = worksheet.GetPrintingPageBreaks(options);

            // Skriv ut information om den första sidbrytningen
            Console.WriteLine($"First page break ends at row: {pageBreaks[0].EndRow}");
        }
    }
}
```

### Se även

* struct [CellArea](../../cellarea/)
* class [ImageOrPrintOptions](../../../aspose.cells.rendering/imageorprintoptions/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


