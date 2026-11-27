---
title: "PivotItem.IsDetailHidden"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotItem-egenskap. Hämtar och anger om detaljen för detta pivot item är dold"
type: docs
url: /sv/net/aspose.cells.pivot/pivotitem/isdetailhidden/
---
## PivotItem.IsDetailHidden property

Hämtar och anger om detaljen för detta pivotelement är dold.

```csharp
public bool IsDetailHidden { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotItemPropertyIsDetailHiddenDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok med exempeldata
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            
            // Lägg till exempeldata för pivottabell
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["A2"].PutValue("Fruit");
            sheet.Cells["A3"].PutValue("Fruit");
            sheet.Cells["A4"].PutValue("Vegetable");
            sheet.Cells["A5"].PutValue("Vegetable");
            sheet.Cells["B1"].PutValue("Item");
            sheet.Cells["B2"].PutValue("Apple");
            sheet.Cells["B3"].PutValue("Orange");
            sheet.Cells["B4"].PutValue("Carrot");
            sheet.Cells["B5"].PutValue("Potato");
            sheet.Cells["C1"].PutValue("Amount");
            sheet.Cells["C2"].PutValue(10);
            sheet.Cells["C3"].PutValue(15);
            sheet.Cells["C4"].PutValue(20);
            sheet.Cells["C5"].PutValue(25);

            // Skapa pivottabell
            int index = sheet.PivotTables.Add("A1:C5", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];
            
            // Lägg till radfält
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Item");
            
            // Lägg till datafält
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Amount");
            
            // Uppdatera och beräkna data
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Dölj detaljer för "Fruit"-kategorin
            pivotTable.RowFields[0].PivotItems["Fruit"].IsDetailHidden = true;
            
            // Spara arbetsboken
            wb.Save("PivotItemIsDetailHiddenDemo.xlsx");
        }
    }
}
```

### Se även

* class [PivotItem](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


