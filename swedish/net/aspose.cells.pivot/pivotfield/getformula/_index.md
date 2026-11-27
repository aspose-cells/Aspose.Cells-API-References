---
title: "PivotField.GetFormula"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotField-metod. Hämtar formeln för det beräknade fältet. Fungerar endast för det beräknade fältet."
type: docs
url: /sv/net/aspose.cells.pivot/pivotfield/getformula/
---
## PivotField.GetFormula method

Hämtar formeln för det beräknade fältet. Fungerar endast för det beräknade fältet.

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
    public class PivotFieldMethodGetFormulaDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok med exempeldata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata för pivottabell
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["A2"].Value = "Bike";
            worksheet.Cells["B2"].Value = 1000;
            worksheet.Cells["A3"].Value = "Car";
            worksheet.Cells["B3"].Value = 2000;
            worksheet.Cells["A4"].Value = "Bike";
            worksheet.Cells["B4"].Value = 1500;
            
            // Skapa pivottabell
            int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            
            // Lägg till beräknat fält med formel
            pivotTable.AddCalculatedField("=ABS('Sales')", "Absolute Sales");
            
            // Hämta formeln från det beräknade fältet
            PivotFieldCollection fields = pivotTable.DataFields;
            string formula = fields[fields.Count - 1].GetFormula();
            
            // Skriv ut formeln
            Console.WriteLine("Calculated field formula: " + formula);
        }
    }
}
```

### Se även

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


