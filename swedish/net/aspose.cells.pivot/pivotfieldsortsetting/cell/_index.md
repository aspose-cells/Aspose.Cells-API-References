---
title: "PivotFieldSortSetting.Cell"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotFieldSortSetting-egenskap. Sorterar efter värdena i vilken rad eller kolumn"
type: docs
url: /sv/net/aspose.cells.pivot/pivotfieldsortsetting/cell/
---
## PivotFieldSortSetting.Cell property

Sorterar efter värdena i vilken rad eller kolumn.

```csharp
public string Cell { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldSortSettingPropertyCellDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok med exempeldata
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata för pivottabell
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Quantity";
            cells["A2"].Value = "Apple";
            cells["A3"].Value = "Orange";
            cells["A4"].Value = "Banana";
            cells["B2"].Value = 10;
            cells["B3"].Value = 5;
            cells["B4"].Value = 8;

            // Skapa pivottabell
            int index = sheet.PivotTables.Add("A1:B4", "D3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Sortera efter cellreferens
            pivotTable.RowFields[0].SortBy(SortOrder.Ascending, 0, PivotLineType.Regular, "A2");
            
            // Demonstrera användning av Cell-egenskapen
            Console.WriteLine("Sorting by cell: " + pivotTable.RowFields[0].SortSetting.Cell);
            
            // Ändra sorteringscell
            pivotTable.RowFields[0].SortBy(SortOrder.Ascending, 0, PivotLineType.Regular, "A3");
            Console.WriteLine("Changed sort cell to: " + pivotTable.RowFields[0].SortSetting.Cell);
            
            // Rensa cellsortering
            pivotTable.RowFields[0].SortBy(SortOrder.Ascending, 0, PivotLineType.GrandTotal, "");
            Console.WriteLine("After clearing cell sort: " + 
                (string.IsNullOrEmpty(pivotTable.RowFields[0].SortSetting.Cell) ? "Empty" : "Has value"));
        }
    }
}
```

### Se även

* class [PivotFieldSortSetting](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


