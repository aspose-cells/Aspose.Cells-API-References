---
title: "Worksheet.StartAccessCache"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Worksheet-metod. Startar sessionen som använder cache för att komma åt data i detta worksheet"
type: docs
url: /sv/net/aspose.cells/worksheet/startaccesscache/
---
## Worksheet.StartAccessCache method

Startar sessionen som använder cache för att komma åt data i detta kalkylblad.

```csharp
public void StartAccessCache(AccessCacheOptions opts)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| opts | AccessCacheOptions | alternativ för dataåtkomst |

### Anmärkningar

Efter att ha avslutat åtkomsten till data bör [`CloseAccessCache`](../closeaccesscache/) anropas med samma alternativ för att rensa alla cacheminnen och återställa normalt åtkomstläge.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodStartAccessCacheWithAccessCacheOptionsDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            
            // Ställ in standardstil
            Style style = wb.DefaultStyle;
            style.Font.Size = 10;
            wb.DefaultStyle = style;

            // Lägg till villkorsstyrd formatering
            ConditionalFormattingCollection cfc = sheet.ConditionalFormattings;
            FormatConditionCollection fcc = cfc[cfc.Add()];
            fcc.AddArea(CellArea.CreateCellArea(0, 0, 10, 10));
            fcc.AddCondition(FormatConditionType.DuplicateValues);
            FormatCondition fc = fcc[0];
            fc.Style.Font.Size = 16;

            // Fyll i lite data
            Cells cells = sheet.Cells;
            for (int i = 0; i < 10; i++)
            {
                cells[0, i].PutValue("A");
                cells[i, 0].PutValue(i);
            }

            // Starta åtkomstcache för bättre prestanda
            sheet.StartAccessCache(AccessCacheOptions.ConditionalFormatting);

            // Verifiera stilar
            for (int i = 0; i < 10; i++)
            {
                Console.WriteLine($"Cell[0,{i}] Font Size: {cells[0, i].GetDisplayStyle().Font.Size}");
                Console.WriteLine($"Cell[{i},0] Font Size: {cells[i, 0].GetDisplayStyle().Font.Size}");
            }

            // Stäng cache när du är klar
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


