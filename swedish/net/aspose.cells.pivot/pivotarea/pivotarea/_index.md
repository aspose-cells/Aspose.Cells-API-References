---
title: "PivotArea.PivotArea"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotArea-konstruktor. Visar det valda området i PivotTable"
type: docs
url: /sv/net/aspose.cells.pivot/pivotarea/pivotarea/
---
## PivotArea constructor

Visar det valda området i pivottabellen.

```csharp
public PivotArea(PivotTable table)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| tabell | PivotTable |  |

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotAreaMethodctorWithPivotTableDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 1000;
            worksheet.Cells["B3"].Value = 2000;

            // Skapa pivottabell
            int pivotIndex = worksheet.PivotTables.Add("=A1:B3", "E5", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // Lägg till fält i pivottabell
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Demonstrera PivotArea-konstruktor med PivotTable-parameter
            PivotArea pivotArea = new PivotArea(pivotTable);
            
            // Konfigurera pivotområde
            pivotArea.AxisType = PivotFieldType.Row;
            pivotArea.RuleType = PivotAreaType.Normal;
            
            // Spara arbetsboken
            workbook.Save("PivotAreaDemo.xlsx");
        }
    }
}
```

### Se även

* class [PivotTable](../../pivottable/)
* class [PivotArea](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


