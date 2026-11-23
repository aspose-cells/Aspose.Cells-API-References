---
title: "Classe SlicerCacheItem"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.Slicers.SlicerCacheItem. Représente un élément de source de données du slicer"
type: docs
url: /fr/net/aspose.cells.slicers/slicercacheitem/
---
## SlicerCacheItem class

Représente l'élément de source de données du slicer

```csharp
public class SlicerCacheItem
```

## Propriétés

| Nom | Description |
| --- | --- |
| [Selected](../../aspose.cells.slicers/slicercacheitem/selected/) { get; set; } | Spécifie si le `SlicerCacheItem` est sélectionné ou non. |
| [Value](../../aspose.cells.slicers/slicercacheitem/value/) { get; } | Renvoie le texte de l'étiquette pour l'élément du slicer. |

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Slicers;

namespace AsposeCellsExamples
{
    public class SlicersClassSlicerCacheItemDemo
    {
        public static void Run()
        {
            // Charger le classeur avec le slicer
            Workbook workbook = new Workbook("example.xlsx");
            workbook.Worksheets.RefreshAll();

            // Obtenir le premier slicer du classeur
            var slicer = workbook.Worksheets
                .SelectMany(x => x.Slicers)
                .First();

            // Itérer à travers les éléments du cache du slicer
            Console.WriteLine("Slicer Cache Items:");
            for (int i = 0; i < slicer.SlicerCache.SlicerCacheItems.Count; i++)
            {
                SlicerCacheItem slicerCacheItem = slicer.SlicerCache.SlicerCacheItems[i];
                Console.WriteLine($"Item {i}: Selected={slicerCacheItem.Selected}, Value={slicerCacheItem.Value}");
            }
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Slicers](../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../)


