---
title: "Enum PivotAreaType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Pivot.PivotAreaType‑enum. Indikerar typen av regel som används för att beskriva ett område eller en aspekt av pivåtabellen"
type: docs
url: /sv/net/aspose.cells.pivot/pivotareatype/
---
## PivotAreaType enumeration

Anger vilken typ av regel som används för att beskriva ett område eller en aspekt av PivotTable.

```csharp
public enum PivotAreaType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| None | `0` | Inget pivåområde. |
| Normal | `1` | Representerar en rubrik eller ett objekt. |
| Data | `2` | Representerar något i dataområdet. |
| All | `3` | Representerar hela pivåtabellen. |
| Origin | `4` | Representerar de tomma cellerna längst upp till vänster i pivottabellen (längst upp till höger för RTL-ark). |
| Button | `5` | Representerar en fältknapp. |
| TopRight | `6` | Representerar de tomma cellerna längst upp till höger i pivottabellen (längst upp till vänster för RTL-ark). |

### Exempel

```csharp
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System;

namespace AsposeCellsExamples
{
    public class PivotAreaTypeDemo
    {
        public static void PivotAreaTypeExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Lägg till ett nytt kalkylblad i arbetsboken
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata i kalkylbladet
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["A2"].PutValue("Apples");
            worksheet.Cells["A3"].PutValue("Oranges");
            worksheet.Cells["A4"].PutValue("Bananas");

            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(150);
            worksheet.Cells["B4"].PutValue(200);

            // Skapa en pivottabell
            int pivotTableIndex = worksheet.PivotTables.Add("=A1:B4", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotTableIndex];

            // Lägg till fält i pivottabellen
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Product
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1); // Sales

            // Skapa ett PivotArea för pivottabellen
            PivotArea pivotArea = new PivotArea(pivotTable);
            pivotArea.RuleType = PivotAreaType.Normal;
            pivotArea.OnlyData = true;
            pivotArea.IsRowGrandIncluded = true;

            // Skriv ut PivotArea-egenskaperna
            Console.WriteLine("Pivot Area Type: " + pivotArea.RuleType);
            Console.WriteLine("Only Data: " + pivotArea.OnlyData);
            Console.WriteLine("Is Row Grand Included: " + pivotArea.IsRowGrandIncluded);

            // Spara arbetsboken
            workbook.Save("PivotAreaTypeExample.xlsx");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


