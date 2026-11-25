---
title: "SlicerCacheItemCollection.Item"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà SlicerCacheItemCollection. Ottiene l'oggetto SlicerCacheItem per indice"
type: docs
url: /it/net/aspose.cells.slicers/slicercacheitemcollection/item/
---
## SlicerCacheItemCollection indexer

Ottiene l'oggetto SlicerCacheItem per indice.

```csharp
public SlicerCacheItem this[int index] { get; }
```

### Esempi

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
            // Crea una cartella di lavoro e aggiungi una tabella pivot
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio
            sheet.Cells["A1"].Value = "Fruit";
            sheet.Cells["A2"].Value = "Apple";
            sheet.Cells["A3"].Value = "Orange";
            sheet.Cells["A4"].Value = "Banana";
            sheet.Cells["B1"].Value = "Sales";
            sheet.Cells["B2"].Value = 100;
            sheet.Cells["B3"].Value = 200;
            sheet.Cells["B4"].Value = 300;

            // Crea tabella pivot
            PivotTableCollection pivotTables = sheet.PivotTables;
            int pivotIndex = pivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = pivotTables[pivotIndex];
            
            // Aggiungi campi alla tabella pivot
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Aggiungi slicer
            SlicerCollection slicers = sheet.Slicers;
            int slicerIndex = slicers.Add(pivotTable, "Fruit", "A1");
            Slicer slicer = slicers[slicerIndex];
            
            // Accedi agli elementi della cache slicer usando la proprietà Item
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

### Vedi anche

* class [SlicerCacheItem](../../slicercacheitem/)
* class [SlicerCacheItemCollection](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)


