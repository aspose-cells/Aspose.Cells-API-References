---
title: "PivotField.SetSubtotals"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotField metod. Anger hur delbelopp ska beräknas för det angivna fältet"
type: docs
url: /sv/net/aspose.cells.pivot/pivotfield/setsubtotals/
---
## PivotField.SetSubtotals method

Anger hur det angivna fältet ska delsummeras.

```csharp
public void SetSubtotals(PivotFieldSubtotalType subtotalType, bool shown)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| subtotalType | PivotFieldSubtotalType | [`PivotFieldSubtotalType`](../../pivotfieldsubtotaltype/) |
| visad | Boolean | Om det angivna fältet visar delsummeringar. |

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldMethodSetSubtotalsWithPivotFieldSubtotalTypeBooleanDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Lägg till exempeldata för pivottabell
            var cells = sheet.Cells;
            cells["A1"].Value = "Category";
            cells["B1"].Value = "Product";
            cells["C1"].Value = "Sales";
            
            cells["A2"].Value = "Electronics";
            cells["B2"].Value = "TV";
            cells["C2"].Value = 1000;
            
            cells["A3"].Value = "Electronics";
            cells["B3"].Value = "Radio";
            cells["C3"].Value = 500;
            
            cells["A4"].Value = "Clothing";
            cells["B4"].Value = "Shirt";
            cells["C4"].Value = 300;
            
            cells["A5"].Value = "Clothing";
            cells["B5"].Value = "Pants";
            cells["C5"].Value = 400;

            // Lägg till pivottabell
            int pivotIndex = sheet.PivotTables.Add("=A1:C5", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[pivotIndex];

            // Lägg till radfält
            int rowIndex = pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            PivotField rowField = pivotTable.RowFields[rowIndex];
            
            // Demonstrera SetSubtotals med PivotFieldSubtotalType och boolesk.
            rowField.SetSubtotals(PivotFieldSubtotalType.Sum, true);

            // Lägg till datafält
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Uppdatera och beräkna pivottabell
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Spara arbetsboken
            workbook.Save("PivotFieldSetSubtotalsDemo.xlsx");
        }
    }
}
```

### Se även

* enum [PivotFieldSubtotalType](../../pivotfieldsubtotaltype/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


