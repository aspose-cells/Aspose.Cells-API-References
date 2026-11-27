---
title: "PageSetup.CustomPaperSize"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PageSetup-metod. Ställer in anpassad papperstorlek i tum"
type: docs
url: /sv/net/aspose.cells/pagesetup/custompapersize/
---
## PageSetup.CustomPaperSize method

Anger den anpassade pappersstorleken i tum.

```csharp
public void CustomPaperSize(double width, double height)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| bredd | Double | Bredden på papperet. |
| höjd | Double | Höjden på papperet. |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupMethodCustomPaperSizeWithDoubleDoubleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ställ in anpassad pappersstorlek (bredd: 1,5 tum, höjd: 1,5 tum)
            worksheet.PageSetup.CustomPaperSize(1.5, 1.5);
            
            // Spara arbetsboken för att demonstrera effekten
            workbook.Save("CustomPaperSizeDemo.xlsx");
        }
    }
}
```

### Se även

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


