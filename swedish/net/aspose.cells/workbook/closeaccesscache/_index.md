---
title: "Workbook.CloseAccessCache"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Workbook-metod. Stänger sessionen som använder cache för att komma åt data"
type: docs
url: /sv/net/aspose.cells/workbook/closeaccesscache/
---
## Workbook.CloseAccessCache method

Stänger sessionen som använder cache för att komma åt data.

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
    public class WorkbookMethodCloseAccessCacheWithAccessCacheOptionsDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Lägg till exempeldata och villkorsstyrd formatering
            for (int i = 0; i < 10; i++)
            {
                cells[i, 0].PutValue(i % 2 == 0 ? "Data" : "Other");
            }

            // Lägg till villkorsstyrd formatering
            int ruleIdx = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = worksheet.ConditionalFormattings[ruleIdx];
            fcc.AddCondition(FormatConditionType.CellValue, OperatorType.Equal, "Data", null);
            Style style = workbook.CreateStyle();
            style.Font.Size = 16;
            fcc.AddArea(new CellArea { StartRow = 0, StartColumn = 0, EndRow = 9, EndColumn = 0 });
            fcc[0].Style = style;

            // Starta åtkomstcache för villkorsstyrd formatering
            workbook.StartAccessCache(AccessCacheOptions.ConditionalFormatting);

            // Kom åt celler med cachad villkorsstyrd formatering
            for (int i = 0; i < 10; i++)
            {
                Cell cell = cells[i, 0];
                Console.WriteLine($"Cell {cell.Name}: Value={cell.StringValue}, FontSize={cell.GetDisplayStyle().Font.Size}");
            }

            // Stäng åtkomstcachen
            workbook.CloseAccessCache(AccessCacheOptions.ConditionalFormatting);

            // Spara arbetsboken
            workbook.Save("output.xlsx");
        }
    }
}
```

### Se även

* enum [AccessCacheOptions](../../accesscacheoptions/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


