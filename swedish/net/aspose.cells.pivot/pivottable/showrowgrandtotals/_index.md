---
title: "PivotTable.ShowRowGrandTotals"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotTable-egenskap. Anger om totalsummor för rader i pivottabellen ska visas"
type: docs
url: /sv/net/aspose.cells.pivot/pivottable/showrowgrandtotals/
---
## PivotTable.ShowRowGrandTotals property

Anger om totalsummor för rader i pivottabellen ska visas.

```csharp
public bool ShowRowGrandTotals { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyShowRowGrandTotalsDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Lägg till ett kalkylblad
            Worksheet sheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata för pivottabell
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Product";
            cells["B1"].Value = "Region";
            cells["C1"].Value = "Sales";
            
            cells["A2"].Value = "Product A";
            cells["B2"].Value = "North";
            cells["C2"].Value = 1000;
            
            cells["A3"].Value = "Product B";
            cells["B3"].Value = "South";
            cells["C3"].Value = 1500;
            
            cells["A4"].Value = "Product A";
            cells["B4"].Value = "South";
            cells["C4"].Value = 2000;
            
            cells["A5"].Value = "Product B";
            cells["B5"].Value = "North";
            cells["C5"].Value = 1200;

            // Lägg till en pivottabell
            PivotTableCollection pivotTables = sheet.PivotTables;
            int index = pivotTables.Add("A1:C5", "E3", "PivotTable1");
            PivotTable pivotTable = pivotTables[index];
            
            // Konfigurera pivottabell
            pivotTable.ShowRowGrandTotals = true; // Demonstrate ShowRowGrandTotals property
            pivotTable.ShowColumnGrandTotals = true;
            
            // Lägg till fält i områden
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Product as row
            pivotTable.AddFieldToArea(PivotFieldType.Column, 1); // Region as column
            pivotTable.AddFieldToArea(PivotFieldType.Data, 2); // Sales as data
            
            // Spara arbetsboken
            workbook.Save("PivotTableShowRowGrandTotalsDemo.xlsx");
        }
    }
}
```

### Se även

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


