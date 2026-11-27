---
title: "PivotItem.Position"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotItem-egenskap. Anger indexet för detta objekt bland alla PivotItems i fältet"
type: docs
url: /sv/net/aspose.cells.pivot/pivotitem/position/
---
## PivotItem.Position property

Anger indexet för detta objekt i alla PivotItems i fältet.

```csharp
public int Position { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotItemPropertyPositionDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok med exempeldata
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata för pivottabell
            sheet.Cells["A1"].PutValue("Product");
            sheet.Cells["B1"].PutValue("Sales");
            sheet.Cells["A2"].PutValue("Apple");
            sheet.Cells["A3"].PutValue("Banana");
            sheet.Cells["A4"].PutValue("Orange");
            sheet.Cells["B2"].PutValue(1000);
            sheet.Cells["B3"].PutValue(2000);
            sheet.Cells["B4"].PutValue(3000);

            // Skapa pivottabell
            int index = sheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];
            
            // Lägg till radfält
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            
            // Lägg till datafält
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Demonstrera Position-egenskapen
            PivotField rowField = pivotTable.RowFields[0];
            foreach (PivotItem item in rowField.PivotItems)
            {
                Console.WriteLine($"Before - Name: {item.Name}, Position: {item.Position}");
                item.Position = 0; // Set position to 0
                Console.WriteLine($"After - Name: {item.Name}, Position: {item.Position}");
            }

            // Uppdatera och beräkna pivottabell
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // Spara arbetsboken
            workbook.Save("PivotItemPositionDemo.xlsx");
        }
    }
}
```

### Se även

* class [PivotItem](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


