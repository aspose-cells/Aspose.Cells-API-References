---
title: "Worksheet.CloseAccessCache"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Worksheet‑metod. Stänger sessionen som använder cache för att komma åt data i detta kalkylblad"
type: docs
url: /sv/net/aspose.cells/worksheet/closeaccesscache/
---
## Worksheet.CloseAccessCache method

Stänger sessionen som använder cache för att komma åt data i detta kalkylblad.

```csharp
public void CloseAccessCache(AccessCacheOptions opts)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| opts | AccessCacheOptions | alternativ för dataåtkomst |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodCloseAccessCacheWithAccessCacheOptionsDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            Cells cells = sheet.Cells;
            
            // Fyll celler med exempeldata
            for (int i = 0; i < 1000; i++)
            {
                cells[i, 0].PutValue(i % 10);
            }

            // Lägg till villkorsstyrd formatering
            FormatConditionCollection fcs = sheet.ConditionalFormattings[sheet.ConditionalFormattings.Add()];
            fcs.AddArea(CellArea.CreateCellArea(0, 0, 999, 0));
            fcs.AddCondition(FormatConditionType.ColorScale);

            // Aktivera åtkomstcache för villkorsstyrd formatering
            sheet.StartAccessCache(AccessCacheOptions.ConditionalFormatting);

            // Utför operationer med cachad åtkomst
            Random random = new Random();
            for (int i = 0; i < 100; i++)
            {
                int r = random.Next(0, 1000);
                var style = cells[r, 0].GetDisplayStyle();
                Console.WriteLine($"Cell ({r},0) style: {style.ForegroundArgbColor:X}");
            }

            // Stäng åtkomstcachen
            sheet.CloseAccessCache(AccessCacheOptions.ConditionalFormatting);
        }
    }
}
```

### Se även

* enum [AccessCacheOptions](../../accesscacheoptions/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


