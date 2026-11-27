---
title: "PivotTable.ShowValuesRow"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotTable-egenskap. Anger om värderadsraden visas"
type: docs
url: /sv/net/aspose.cells.pivot/pivottable/showvaluesrow/
---
## PivotTable.ShowValuesRow property

Anger om värderadsrad visas.

```csharp
public bool ShowValuesRow { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyShowValuesRowDemo
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
            cells["B2"].Value = 10;
            cells["A3"].Value = "Orange";
            cells["B3"].Value = 15;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 20;

            // Skapa pivottabell
            int index = sheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];
            
            // Konfigurera pivottabell
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Fruit as row
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1); // Quantity as data
            
            // Demonstrera ShowValuesRow-egenskapen
            Console.WriteLine("Initial ShowValuesRow: " + pivotTable.ShowValuesRow);
            pivotTable.ShowValuesRow = true;
            Console.WriteLine("After setting to true: " + pivotTable.ShowValuesRow);
            
            // Spara arbetsboken
            workbook.Save("PivotTableShowValuesRowDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Se även

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


