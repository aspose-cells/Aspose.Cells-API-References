---
title: "PivotTable.RefreshDate"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotTable‑egenskap. Hämtar det senaste datumet och tiden då pivottabellen uppdaterades"
type: docs
url: /sv/net/aspose.cells.pivot/pivottable/refreshdate/
---
## PivotTable.RefreshDate property

Hämtar det senaste datumet och tiden då PivotTable uppdaterades.

```csharp
public DateTime RefreshDate { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyRefreshDateDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok med exempeldata
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            
            // Lägg till exempeldata för pivottabell
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Quantity";
            cells["A2"].Value = "Apple";
            cells["B2"].Value = 10;
            cells["A3"].Value = "Orange";
            cells["B3"].Value = 15;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 8;

            // Lägg till en pivottabell
            int index = sheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pt = sheet.PivotTables[index];
            
            // Uppdatera pivottabellen för att ange uppdateringsdatum
            pt.RefreshData();
            pt.CalculateData();

            // Visa information om uppdateringsdatum
            Console.WriteLine("Pivot Table Refresh Date: " + pt.RefreshDate.ToLongDateString());
            Console.WriteLine("Refreshed By: " + pt.RefreshedByWho);

            // Spara och ladda om för att demonstrera beständighet
            string savePath = "PivotTableRefreshDateDemo_Out.xlsx";
            wb.Save(savePath);
            
            // Läs om och visa uppdateringsdatum igen
            Workbook wb2 = new Workbook(savePath);
            PivotTable pt2 = wb2.Worksheets[0].PivotTables[0];
            Console.WriteLine("\nAfter reloading:");
            Console.WriteLine("Pivot Table Refresh Date: " + pt2.RefreshDate.ToLongDateString());
        }
    }
}
```

### Se även

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


