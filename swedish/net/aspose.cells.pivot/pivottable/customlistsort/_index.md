---
title: "PivotTable.CustomListSort"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotTable-egenskap. Anger om den inbyggda anpassade listan ska beaktas vid sortering av data"
type: docs
url: /sv/net/aspose.cells.pivot/pivottable/customlistsort/
---
## PivotTable.CustomListSort property

Anger om inbyggda anpassade listor ska beaktas vid sortering av data.

```csharp
public bool CustomListSort { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyCustomListSortDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Lägg till exempeldata för pivottabell
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Quantity";
            cells["A2"].Value = "Apple";
            cells["B2"].Value = 10;
            cells["A3"].Value = "Orange";
            cells["B3"].Value = 20;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 15;
            cells["A5"].Value = "Pear";
            cells["B5"].Value = 5;

            // Skapa pivottabell
            int index = sheet.PivotTables.Add("A1:B5", "C3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];

            // Lägg till radfält och datafält
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");

            // Aktivera sortering av anpassad lista
            pivotTable.CustomListSort = true;

            // Spara arbetsboken
            workbook.Save("PivotTable_CustomListSort_Example.xlsx");
        }
    }
}
```

### Se även

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


