---
title: "SheetPrintingPreview.EvaluatedPageCount"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SheetPrintingPreview-egenskap. Beräkna det totala sidantalet för detta arbetsblad"
type: docs
url: /sv/net/aspose.cells.rendering/sheetprintingpreview/evaluatedpagecount/
---
## SheetPrintingPreview.EvaluatedPageCount property

Utvärdera det totala sidantalet i detta kalkylblad

```csharp
public int EvaluatedPageCount { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class SheetPrintingPreviewPropertyEvaluatedPageCountDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata i kalkylbladet
            for (int i = 0; i < 100; i++)
            {
                worksheet.Cells[i, 0].Value = "Row " + (i + 1);
            }

            ImageOrPrintOptions options = new ImageOrPrintOptions();
            SheetPrintingPreview preview = new SheetPrintingPreview(worksheet, options);
            
            Console.WriteLine("Evaluated Page Count: " + preview.EvaluatedPageCount);
        }
    }
}
```

### Se även

* class [SheetPrintingPreview](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


