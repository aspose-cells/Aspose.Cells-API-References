---
title: "PivotTable.AllowMultipleFiltersPerField"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotTable-egenskap. Anger ett booleskt värde som visar om fälten i en PivotTable kan ha flera filter inställda på dem"
type: docs
url: /sv/net/aspose.cells.pivot/pivottable/allowmultiplefiltersperfield/
---
## PivotTable.AllowMultipleFiltersPerField property

Anger ett booleskt värde som visar om fälten i en PivotTable kan ha flera filter inställda på dem.

```csharp
public bool AllowMultipleFiltersPerField { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyAllowMultipleFiltersPerFieldDemo
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
            cells["A5"].Value = "Apple";
            cells["B5"].Value = 5;
            cells["A6"].Value = "Orange";
            cells["B6"].Value = 10;

            // Skapa pivottabell
            int index = sheet.PivotTables.Add("A1:B6", "C3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];

            // Lägg till fält i pivottabell
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");

            // Ställ in AllowMultipleFiltersPerField-egenskapen
            pivotTable.AllowMultipleFiltersPerField = true;
            Console.WriteLine("AllowMultipleFiltersPerField: " + pivotTable.AllowMultipleFiltersPerField);

            // Spara arbetsboken
            workbook.Save("PivotTable_AllowMultipleFiltersPerField.xlsx");
        }
    }
}
```

### Se även

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


