---
title: "SlicerCacheItem.Value"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SlicerCacheItem-egenskap. Returnerar etiketttexten för slicer-objektet"
type: docs
url: /sv/net/aspose.cells.slicers/slicercacheitem/value/
---
## SlicerCacheItem.Value property

Returnerar etiketttexten för skärmningsobjektet.

```csharp
public string Value { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Slicers;

namespace AsposeCellsExamples
{
    public class SlicerCacheItemPropertyValueDemo
    {
        public static void Run()
        {
            // Skapa arbetsbok med exempeldata
            Workbook wb = new Workbook();
            Worksheet ws = wb.Worksheets[0];
            
            // Skapa exempeldata för pivottabell
            ws.Cells["A1"].PutValue("Name");
            ws.Cells["A2"].PutValue("Alex");
            ws.Cells["A3"].PutValue("Sam");
            ws.Cells["A4"].PutValue("Alex");
            ws.Cells["A5"].PutValue("John");
            
            // Skapa pivottabell
            int index = ws.PivotTables.Add("A1:A5", "E1", "PivotTable1");
            PivotTable pt = ws.PivotTables[index];
            pt.AddFieldToArea(PivotFieldType.Row, "Name");
            
            // Lägg till skärmningskontrollen
            int slicerIndex = ws.Slicers.Add(pt, "Name", "Slicer1");
            Slicer slicer = ws.Slicers[slicerIndex];
            
            // Demonstrera användning av Value‑egenskapen
            Console.WriteLine("All items:");
            foreach (SlicerCacheItem item in slicer.SlicerCache.SlicerCacheItems)
            {
                Console.WriteLine(item.Value);
            }
            
            // Välj endast "Alex"
            Console.WriteLine("\nSelecting only Alex:");
            foreach (SlicerCacheItem item in slicer.SlicerCache.SlicerCacheItems)
            {
                item.Selected = (item.Value == "Alex");
            }
            slicer.Refresh();
            
            // Visa valda objekt
            Console.WriteLine("\nSelected items:");
            foreach (SlicerCacheItem item in slicer.SlicerCache.SlicerCacheItems)
            {
                if (item.Selected)
                {
                    Console.WriteLine(item.Value);
                }
            }
            
            // Välj alla objekt
            Console.WriteLine("\nSelecting all items:");
            foreach (SlicerCacheItem item in slicer.SlicerCache.SlicerCacheItems)
            {
                item.Selected = true;
            }
            slicer.Refresh();
        }
    }
}
```

### Se även

* class [SlicerCacheItem](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)


