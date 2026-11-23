---
title: "SlicerCacheItemCollection.Item"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété SlicerCacheItemCollection. Obtient l’objet SlicerCacheItem par indice"
type: docs
url: /fr/net/aspose.cells.slicers/slicercacheitemcollection/item/
---
## SlicerCacheItemCollection indexer

Obtient l'objet SlicerCacheItem par indice.

```csharp
public SlicerCacheItem this[int index] { get; }
```

### Exemples

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
            // Créer un classeur et ajouter un tableau croisé dynamique
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Ajoutez des données d'exemple
            sheet.Cells["A1"].Value = "Fruit";
            sheet.Cells["A2"].Value = "Apple";
            sheet.Cells["A3"].Value = "Orange";
            sheet.Cells["A4"].Value = "Banana";
            sheet.Cells["B1"].Value = "Sales";
            sheet.Cells["B2"].Value = 100;
            sheet.Cells["B3"].Value = 200;
            sheet.Cells["B4"].Value = 300;

            // Créer un tableau croisé dynamique
            PivotTableCollection pivotTables = sheet.PivotTables;
            int pivotIndex = pivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = pivotTables[pivotIndex];
            
            // Ajouter des champs au tableau croisé dynamique
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Ajouter un slicer
            SlicerCollection slicers = sheet.Slicers;
            int slicerIndex = slicers.Add(pivotTable, "Fruit", "A1");
            Slicer slicer = slicers[slicerIndex];
            
            // Accéder aux éléments du cache de segment en utilisant la propriété Item
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

### Voir aussi

* class [SlicerCacheItem](../../slicercacheitem/)
* class [SlicerCacheItemCollection](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)


