---
title: "PivotField.IsAutoSubtotals"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotField egenskap. Anger om det angivna fältet visar automatiska delsummeringar. Standard är sant."
type: docs
url: /sv/net/aspose.cells.pivot/pivotfield/isautosubtotals/
---
## PivotField.IsAutoSubtotals property

Anger om det angivna fältet visar automatiska delsummer. Standard är true.

```csharp
public bool IsAutoSubtotals { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyIsAutoSubtotalsDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["A2"].Value = "Bikes";
            worksheet.Cells["A3"].Value = "Bikes";
            worksheet.Cells["A4"].Value = "Cars";
            worksheet.Cells["A5"].Value = "Cars";
            worksheet.Cells["B2"].Value = 1000;
            worksheet.Cells["B3"].Value = 2000;
            worksheet.Cells["B4"].Value = 3000;
            worksheet.Cells["B5"].Value = 4000;

            // Skapa pivottabell
            int pivotIndex = worksheet.PivotTables.Add("A1:B5", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Lägg till fält i radområdet och sätt IsAutoSubtotals till falskt
            int fieldIndex = pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            PivotField rowField = pivotTable.RowFields[fieldIndex];
            rowField.IsAutoSubtotals = false; // Disable automatic subtotals

            // Lägg till fält i dataområdet
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Beräkna data
            pivotTable.CalculateData();
            
            // Spara arbetsboken
            workbook.Save("PivotFieldIsAutoSubtotalsDemo.xlsx");
        }
    }
}
```

### Se även

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


