---
title: "PivotField.IsCalculatedField"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotField egenskap. Anger om detta pivottfält är ett beräknat fält"
type: docs
url: /sv/net/aspose.cells.pivot/pivotfield/iscalculatedfield/
---
## PivotField.IsCalculatedField property

Anger om detta pivotfält är ett beräknat fält.

```csharp
public bool IsCalculatedField { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyIsCalculatedFieldDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok med exempeldata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata för pivottabell
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["B2"].Value = 1000;
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["B3"].Value = 2000;
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B4"].Value = 3000;

            // Lägg till en pivottabell
            int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            
            // Lägg till beräknat fält
            pivotTable.AddCalculatedField("Profit", "Sales*0.2", true);

            // Kontrollera om fältet är ett beräknat fält
            PivotField profitField = pivotTable.BaseFields[pivotTable.BaseFields.Count - 1];
            Console.WriteLine("Is Profit field calculated? " + profitField.IsCalculatedField);

            // Spara arbetsboken
            workbook.Save("PivotField_IsCalculatedField_Example.xlsx");
        }
    }
}
```

### Se även

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


