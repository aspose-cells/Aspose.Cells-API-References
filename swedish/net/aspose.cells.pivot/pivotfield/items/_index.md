---
title: "PivotField.Items"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotField-egenskap. Hämtar alla etiketter för pivotelement i detta fält"
type: docs
url: /sv/net/aspose.cells.pivot/pivotfield/items/
---
## PivotField.Items property

Hämta alla etiketter för pivotobjekt i detta fält.

```csharp
public string[] Items { get; }
```

### Exempel

```csharp
using System;
using System.Collections;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyItemsDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok och lägg till exempeldata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata för pivottabell
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["A5"].Value = "Apple";
            worksheet.Cells["B1"].Value = "Quantity";
            worksheet.Cells["B2"].Value = 10;
            worksheet.Cells["B3"].Value = 15;
            worksheet.Cells["B4"].Value = 20;
            worksheet.Cells["B5"].Value = 5;

            // Skapa pivottabell
            int index = worksheet.PivotTables.Add("A1:B5", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            
            // Lägg till pivottfält
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            PivotField pivotField = pivotTable.RowFields[0];
            
            // Demonstrera Items-egenskapen
            string[] items = pivotField.Items;
            Console.WriteLine("Pivot Field Items:");
            foreach (string item in items)
            {
                Console.WriteLine(item);
            }
            
            // Ställ in aktuellt sidobjekt
            ArrayList list = new ArrayList(items);
            if (list.Contains("Apple"))
            {
                pivotField.CurrentPageItem = (short)list.IndexOf("Apple");
                Console.WriteLine("Current page item set to: Apple");
            }
            
            pivotTable.CalculateData();
        }
    }
}
```

### Se även

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


