---
title: "PivotTable.ShowPivotStyleLastColumn"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotTable-egenskap. Anger om kolumnformateringen tillämpas"
type: docs
url: /sv/net/aspose.cells.pivot/pivottable/showpivotstylelastcolumn/
---
## PivotTable.ShowPivotStyleLastColumn property

Anger om kolumnformatering har tillämpats.

```csharp
public bool ShowPivotStyleLastColumn { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyShowPivotStyleLastColumnDemo
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
            cells["B3"].Value = 15;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 20;

            // Skapa pivottabell
            int index = sheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];

            // Ställ in pivottabellens stil och visa stil för sista kolumnen
            pivotTable.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium9;
            pivotTable.ShowPivotStyleLastColumn = true;

            // Spara arbetsboken
            workbook.Save("PivotTableShowLastColumnStyle.xlsx");
        }
    }
}
```

### Se även

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


