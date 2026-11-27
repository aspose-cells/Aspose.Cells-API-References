---
title: "SlicerCacheItem.Selected"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SlicerCacheItem-egenskap. Anger om SlicerCacheItem är markerad eller inte"
type: docs
url: /sv/net/aspose.cells.slicers/slicercacheitem/selected/
---
## SlicerCacheItem.Selected property

Anger om [`SlicerCacheItem`](../) är markerad eller inte.

```csharp
public bool Selected { get; set; }
```

### Anmärkningar

Använd istället [`SelectItems`](../../slicer/selectitems/)‑metoden om du vill markera ett objekt. Detta uppdateringsförfarande ger dålig prestanda på grund av fullständig dataomladdning varje gång markeringen ändras.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Slicers;

namespace AsposeCellsExamples
{
    public class SlicerCacheItemPropertySelectedDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok med exempeldata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Skapa exempeldata för pivottabell
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 100;
            worksheet.Cells["B3"].Value = 200;
            worksheet.Cells["B4"].Value = 300;

            // Skapa pivottabell
            int index = worksheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Lägg till skärmningskontrollen
            int slicerIndex = worksheet.Slicers.Add(pivotTable, "Fruit", "Slicer1");
            Aspose.Cells.Slicers.Slicer slicer = worksheet.Slicers[slicerIndex];
            slicer.StyleType = SlicerStyleType.SlicerStyleLight1;

            // Åtkomst till slicer-cache-objekt
            for (int i = 0; i < slicer.SlicerCache.SlicerCacheItems.Count; i++)
            {
                SlicerCacheItem item = slicer.SlicerCache.SlicerCacheItems[i];
                
                // Välj första objektet, avmarkera övriga
                if (i == 0)
                {
                    item.Selected = true;
                    Console.WriteLine($"Item '{item.Value}' is selected: {item.Selected}");
                }
                else
                {
                    item.Selected = false;
                    Console.WriteLine($"Item '{item.Value}' is selected: {item.Selected}");
                }
            }

            // Spara arbetsboken
            workbook.Save("SlicerCacheItemSelectedDemo.xlsx");
        }
    }
}
```

### Se även

* class [SlicerCacheItem](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)


