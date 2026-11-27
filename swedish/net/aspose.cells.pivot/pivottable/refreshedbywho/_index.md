---
title: "PivotTable.RefreshedByWho"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotTable-egenskap. Hämtar namnet på den senaste användaren som uppdaterade denna PivotTable"
type: docs
url: /sv/net/aspose.cells.pivot/pivottable/refreshedbywho/
---
## PivotTable.RefreshedByWho property

Hämtar namnet på den senaste användaren som uppdaterade denna PivotTable

```csharp
public string RefreshedByWho { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyRefreshedByWhoDemo
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

            // Skapa pivottabell
            int pivotIndex = sheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pt = sheet.PivotTables[pivotIndex];
            
            // Lägg till fält i pivottabell
            pt.AddFieldToArea(PivotFieldType.Row, 0);
            pt.AddFieldToArea(PivotFieldType.Data, 1);
            
            // Uppdatera pivottabellen för att sätta RefreshedByWho-egenskapen
            pt.RefreshData();
            pt.CalculateData();

            // Skriv ut uppdateringsinformation
            Console.WriteLine("Pivot Table Refresh Information:");
            Console.WriteLine("Last Refresh Date: " + pt.RefreshDate);
            Console.WriteLine("Refreshed By: " + pt.RefreshedByWho);
            
            // Spara och ladda om för att demonstrera egenskapsbeständighet
            string savePath = "PivotTableRefreshedByWhoDemo_Out.xlsx";
            wb.Save(savePath);
            
            // Ladda om arbetsboken och kontrollera egenskapen
            Workbook wb2 = new Workbook(savePath);
            PivotTable pt2 = wb2.Worksheets[0].PivotTables[0];
            Console.WriteLine("\nAfter Reload:");
            Console.WriteLine("Last Refresh Date: " + pt2.RefreshDate);
            Console.WriteLine("Refreshed By: " + pt2.RefreshedByWho);
        }
    }
}
```

### Se även

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


