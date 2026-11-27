---
title: "PivotTable.ShowColumnGrandTotals"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotTable-egenskap. Anger om sammanlagda totaler för kolumner i denna pivottabell ska visas"
type: docs
url: /sv/net/aspose.cells.pivot/pivottable/showcolumngrandtotals/
---
## PivotTable.ShowColumnGrandTotals property

Anger om totalsummor för kolumner i denna pivottabell ska visas.

```csharp
public bool ShowColumnGrandTotals { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyShowColumnGrandTotalsDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Lägg till exempeldata för pivottabell
            var cells = sheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Quantity";
            cells["A2"].Value = "Apple";
            cells["A3"].Value = "Orange";
            cells["A4"].Value = "Banana";
            cells["A5"].Value = "Apple";
            cells["B2"].Value = 5;
            cells["B3"].Value = 3;
            cells["B4"].Value = 6;
            cells["B5"].Value = 2;

            // Lägg till pivottabell
            int index = sheet.PivotTables.Add("A1:B5", "C3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];

            // Konfigurera pivottabell
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Fruit as rows
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1); // Sum of Quantity

            // Demonstrera egenskapen ShowColumnGrandTotals
            pivotTable.ShowColumnGrandTotals = false; // Disable column grand totals
            Console.WriteLine("Column Grand Totals Visible: " + pivotTable.ShowColumnGrandTotals);

            // Spara arbetsboken
            workbook.Save("PivotTableShowColumnGrandTotalsDemo.xlsx");
        }
    }
}
```

### Se även

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


