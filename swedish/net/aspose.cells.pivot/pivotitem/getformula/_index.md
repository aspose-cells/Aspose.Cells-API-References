---
title: "PivotItem.GetFormula"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotItem-metod. Hämtar formeln för detta beräknade objekt. Fungerar endast när objektet är ett beräknat objekt"
type: docs
url: /sv/net/aspose.cells.pivot/pivotitem/getformula/
---
## PivotItem.GetFormula method

Hämtar formeln för detta beräknade objekt. Fungerar endast när detta objekt är ett beräknat objekt.

```csharp
public string GetFormula()
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotItemMethodGetFormulaDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok med exempeldata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata för pivottabell
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 100;
            worksheet.Cells["B3"].Value = 150;
            worksheet.Cells["B4"].Value = 200;

            // Lägg till en pivottabell
            int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            
            // Lägg till radfält och datafält
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
            
            // Beräkna data
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Hämta formel från pivot-element
            string rowItemFormula = pivotTable.RowFields[0].PivotItems[0].GetFormula();
            string dataFieldFormula = pivotTable.DataFields[0].GetFormula();

            Console.WriteLine("Row Item Formula: " + rowItemFormula);
            Console.WriteLine("Data Field Formula: " + dataFieldFormula);
        }
    }
}
```

### Se även

* class [PivotItem](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


