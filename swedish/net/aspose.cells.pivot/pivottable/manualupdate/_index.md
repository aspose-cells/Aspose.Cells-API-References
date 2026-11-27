---
title: "PivotTable.ManualUpdate"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotTable-egenskap. Anger om pivottabellrapporten endast beräknas om användaren begär det"
type: docs
url: /sv/net/aspose.cells.pivot/pivottable/manualupdate/
---
## PivotTable.ManualUpdate property

Anger om PivotTable‑rapporten beräknas om endast på begäran av användaren.

```csharp
public bool ManualUpdate { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyManualUpdateDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok
            Workbook workbook = new Workbook();
            
            // Lägg till ett kalkylblad och fyll i med exempeldata
            Worksheet dataSheet = workbook.Worksheets["Sheet1"];
            dataSheet.Cells["A1"].PutValue("Category");
            dataSheet.Cells["B1"].PutValue("Value");
            dataSheet.Cells["A2"].PutValue("A");
            dataSheet.Cells["B2"].PutValue(10);
            dataSheet.Cells["A3"].PutValue("B");
            dataSheet.Cells["B3"].PutValue(20);
            dataSheet.Cells["A4"].PutValue("A");
            dataSheet.Cells["B4"].PutValue(30);

            // Lägg till en pivottabell
            Worksheet pivotSheet = workbook.Worksheets.Add("PivotSheet");
            int index = pivotSheet.PivotTables.Add("Sheet1!A1:B4", "A3", "PivotTable1");
            PivotTable pivotTable = pivotSheet.PivotTables[index];

            // Konfigurera pivottabell
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Value");
            
            // Aktivera manuell uppdatering
            pivotTable.ManualUpdate = true;
            
            // Vid det här tillfället uppdateras inte pivottabellen automatiskt
            Console.WriteLine("Pivot table before refresh (ManualUpdate=true):");
            Console.WriteLine(pivotSheet.Cells["B4"].StringValue); // Will be empty
            
            // Uppdatera pivottabellen manuellt
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            Console.WriteLine("Pivot table after manual refresh:");
            Console.WriteLine(pivotSheet.Cells["B4"].StringValue); // Will show "40" (sum of category A)
            
            // Spara arbetsboken
            workbook.Save("PivotTableManualUpdateDemo.xlsx");
        }
    }
}
```

### Se även

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


