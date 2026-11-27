---
title: "PivotTable.SubtotalHiddenPageItems"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotTable-egenskap. Anger om dolda sidfältselement i PivotTable-rapporten inkluderas i rad- och kolumnsubtotaler, blocktotaler och totalsummor. Standardvärdet är False"
type: docs
url: /sv/net/aspose.cells.pivot/pivottable/subtotalhiddenpageitems/
---
## PivotTable.SubtotalHiddenPageItems property

Anger om dolda sidfältsposter i PivotTable‑rapporten inkluderas i rad‑ och kolumnsubtotals, block‑totals och totalsummor. Standardvärdet är False.

```csharp
public bool SubtotalHiddenPageItems { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertySubtotalHiddenPageItemsDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Lägg till exempeldata för pivottabell
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Region";
            cells["C1"].Value = "Sales";
            
            cells["A2"].Value = "Apple";
            cells["B2"].Value = "North";
            cells["C2"].Value = 1000;
            
            cells["A3"].Value = "Orange";
            cells["B3"].Value = "South";
            cells["C3"].Value = 2000;
            
            cells["A4"].Value = "Banana";
            cells["B4"].Value = "North";
            cells["C4"].Value = 1500;
            
            cells["A5"].Value = "Apple";
            cells["B5"].Value = "South";
            cells["C5"].Value = 1200;

            // Skapa pivottabell
            int index = sheet.PivotTables.Add("A1:C5", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];
            
            // Lägg till fält
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Column, "Region");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Ställ in egenskapen SubtotalHiddenPageItems
            pivotTable.SubtotalHiddenPageItems = true;
            Console.WriteLine("SubtotalHiddenPageItems set to: " + pivotTable.SubtotalHiddenPageItems);

            // Uppdatera och beräkna data
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Spara arbetsboken
            workbook.Save("PivotTable_SubtotalHiddenPageItemsDemo.xlsx");
        }
    }
}
```

### Se även

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


