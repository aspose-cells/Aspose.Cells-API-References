---
title: "SlicerCacheItem.Value"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété SlicerCacheItem. Retourne le texte d'étiquette pour l'élément de segment"
type: docs
url: /fr/net/aspose.cells.slicers/slicercacheitem/value/
---
## SlicerCacheItem.Value property

Renvoie le texte de l'étiquette pour l'élément du slicer.

```csharp
public string Value { get; }
```

### Exemples

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
            // Créer un classeur avec des données d'exemple
            Workbook wb = new Workbook();
            Worksheet ws = wb.Worksheets[0];
            
            // Créer des données d'exemple pour le tableau croisé dynamique
            ws.Cells["A1"].PutValue("Name");
            ws.Cells["A2"].PutValue("Alex");
            ws.Cells["A3"].PutValue("Sam");
            ws.Cells["A4"].PutValue("Alex");
            ws.Cells["A5"].PutValue("John");
            
            // Créer un tableau croisé dynamique
            int index = ws.PivotTables.Add("A1:A5", "E1", "PivotTable1");
            PivotTable pt = ws.PivotTables[index];
            pt.AddFieldToArea(PivotFieldType.Row, "Name");
            
            // Ajouter un slicer
            int slicerIndex = ws.Slicers.Add(pt, "Name", "Slicer1");
            Slicer slicer = ws.Slicers[slicerIndex];
            
            // Démontrez l'utilisation de la propriété Value
            Console.WriteLine("All items:");
            foreach (SlicerCacheItem item in slicer.SlicerCache.SlicerCacheItems)
            {
                Console.WriteLine(item.Value);
            }
            
            // Sélectionner uniquement "Alex"
            Console.WriteLine("\nSelecting only Alex:");
            foreach (SlicerCacheItem item in slicer.SlicerCache.SlicerCacheItems)
            {
                item.Selected = (item.Value == "Alex");
            }
            slicer.Refresh();
            
            // Afficher les éléments sélectionnés
            Console.WriteLine("\nSelected items:");
            foreach (SlicerCacheItem item in slicer.SlicerCache.SlicerCacheItems)
            {
                if (item.Selected)
                {
                    Console.WriteLine(item.Value);
                }
            }
            
            // Sélectionner tous les éléments
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

### Voir aussi

* class [SlicerCacheItem](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)


