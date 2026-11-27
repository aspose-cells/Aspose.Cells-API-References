---
title: "HorizontalPageBreak.Row"
second_title: "Aspose.Cells för .NET API‑referens"
description: "HorizontalPageBreak property. Hämtar det nollbaserade radindexet"
type: docs
url: /sv/net/aspose.cells/horizontalpagebreak/row/
---
## HorizontalPageBreak.Row property

Hämtar radindex med nollbas.

```csharp
public int Row { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HorizontalPageBreakPropertyRowDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till horisontella sidbrytningar
            worksheet.HorizontalPageBreaks.Add(6);
            worksheet.HorizontalPageBreaks.Add(12);

            // Hämta samlingen av horisontella sidbrytningar
            HorizontalPageBreakCollection breaks = worksheet.HorizontalPageBreaks;

            // Visa radnummer för sidbrytningar
            Console.WriteLine("Page break at row: " + breaks[0].Row);
            Console.WriteLine("Page break at row: " + breaks[1].Row);

            // Spara arbetsboken
            workbook.Save("output.xlsx");
        }
    }
}
```

### Se även

* class [HorizontalPageBreak](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


