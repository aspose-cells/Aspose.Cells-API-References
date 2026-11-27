---
title: "PivotItem.Name"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotItem-egenskap. Hämtar namnet på pivot-elementet"
type: docs
url: /sv/net/aspose.cells.pivot/pivotitem/name/
---
## PivotItem.Name property

Hämtar namnet på pivotobjektet.

```csharp
public string Name { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotItemPropertyNameDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok med exempeldata
            Workbook wb = new Workbook();
            Worksheet ws = wb.Worksheets[0];
            
            // Lägg till exempeldata för pivottabell
            ws.Cells["A1"].Value = "Category";
            ws.Cells["B1"].Value = "Value";
            ws.Cells["A2"].Value = "债券借贷";
            ws.Cells["A3"].Value = "股票";
            ws.Cells["A4"].Value = "基金";
            ws.Cells["B2"].Value = 100;
            ws.Cells["B3"].Value = 200;
            ws.Cells["B4"].Value = 300;

            // Skapa pivottabell
            int index = ws.PivotTables.Add("A1:B4", "D3", "PivotTable1");
            PivotTable pivotTable = ws.PivotTables[index];
            
            // Lägg till radfält
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            
            // Lägg till datafält
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Value");
            
            // Få åtkomst till pivot-element och demonstrera Name-egenskapen
            PivotField field = pivotTable.RowFields[0];
            foreach (PivotItem item in field.PivotItems)
            {
                // Dölj alla element förutom "债券借贷"
                item.IsHidden = item.Name != "债券借贷";
                Console.WriteLine($"Pivot Item Name: {item.Name}, Hidden: {item.IsHidden}");
            }
            
            // Uppdatera och spara
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            wb.Save("PivotItemNameDemo.xlsx");
        }
    }
}
```

### Se även

* class [PivotItem](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


