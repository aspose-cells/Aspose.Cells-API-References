---
title: "SlicerCacheItemCollection.Item"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "SlicerCacheItemCollection‑Eigenschaft. Gibt das SlicerCacheItem‑Objekt anhand des Index zurück"
type: docs
url: /de/net/aspose.cells.slicers/slicercacheitemcollection/item/
---
## SlicerCacheItemCollection indexer

Liefert das SlicerCacheItem‑Objekt nach Index.

```csharp
public SlicerCacheItem this[int index] { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Slicers;

namespace AsposeCellsExamples
{
    public class SlicerCacheItemCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Erstelle eine Arbeitsmappe und füge eine Pivot‑Tabelle hinzu
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Fügen Sie Beispieldaten hinzu
            sheet.Cells["A1"].Value = "Fruit";
            sheet.Cells["A2"].Value = "Apple";
            sheet.Cells["A3"].Value = "Orange";
            sheet.Cells["A4"].Value = "Banana";
            sheet.Cells["B1"].Value = "Sales";
            sheet.Cells["B2"].Value = 100;
            sheet.Cells["B3"].Value = 200;
            sheet.Cells["B4"].Value = 300;

            // Pivot-Tabelle erstellen
            PivotTableCollection pivotTables = sheet.PivotTables;
            int pivotIndex = pivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = pivotTables[pivotIndex];
            
            // Felder zur Pivot-Tabelle hinzufügen
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Füge Slicer hinzu
            SlicerCollection slicers = sheet.Slicers;
            int slicerIndex = slicers.Add(pivotTable, "Fruit", "A1");
            Slicer slicer = slicers[slicerIndex];
            
            // Greife auf Slicer‑Cache‑Elemente über die Item‑Eigenschaft zu
            SlicerCacheItemCollection items = slicer.SlicerCache.SlicerCacheItems;
            if (items.Count > 0)
            {
                SlicerCacheItem item = items[0]; // Demonstrating Item property usage
                Console.WriteLine("First slicer item: " + item.Value);
            }
        }
    }
}
```

### Siehe auch

* class [SlicerCacheItem](../../slicercacheitem/)
* class [SlicerCacheItemCollection](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)


