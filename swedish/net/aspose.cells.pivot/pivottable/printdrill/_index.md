---
title: "PivotTable.PrintDrill"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotTable-egenskap. Anger ett booleskt värde som visar om borrindikatorer ska skrivas ut. Skriv ut expandera/kollapsa-knappar när de visas på pivottabellen"
type: docs
url: /sv/net/aspose.cells.pivot/pivottable/printdrill/
---
## PivotTable.PrintDrill property

Anger ett booleskt värde som visar om drill‑indikatorer ska skrivas ut. Skriv ut expandera/komprimera‑knappar när de visas i pivottabellen.

```csharp
public bool PrintDrill { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyPrintDrillDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            var cells = sheet.Cells;
            cells["A1"].Value = "Product";
            cells["B1"].Value = "Sales";
            cells["A2"].Value = "Bikes";
            cells["B2"].Value = 1000;
            cells["A3"].Value = "Cars";
            cells["B3"].Value = 2000;
            cells["A4"].Value = "Bikes";
            cells["B4"].Value = 1500;
            cells["A5"].Value = "Cars";
            cells["B5"].Value = 2500;

            // Lägg till en pivottabell
            int index = sheet.PivotTables.Add("A1:B5", "D1", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];

            // Konfigurera pivottabell
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Demonstrera PrintDrill-egenskapen
            pivotTable.PrintDrill = false; // Disable printing drill indicators
            pivotTable.ShowDrill = true;   // Show drill indicators on screen
            
            // Uppdatera och beräkna pivottabell
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Spara arbetsboken
            workbook.Save("PivotTablePrintDrillDemo.xlsx");
        }
    }
}
```

### Se även

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


