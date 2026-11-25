---
title: "Classe SlicerCacheItem"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.Slicers.SlicerCacheItem. Rappresenta l'elemento della fonte dati dello slicer"
type: docs
url: /it/net/aspose.cells.slicers/slicercacheitem/
---
## SlicerCacheItem class

Rappresenta l'elemento della fonte dati dello slicer

```csharp
public class SlicerCacheItem
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Selected](../../aspose.cells.slicers/slicercacheitem/selected/) { get; set; } | Specifica se il `SlicerCacheItem` è selezionato o meno. |
| [Value](../../aspose.cells.slicers/slicercacheitem/value/) { get; } | Restituisce il testo dell'etichetta per l'elemento dello slicer. |

### Esempi

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
            // Carica la cartella di lavoro con lo slicer
            Workbook workbook = new Workbook("example.xlsx");
            workbook.Worksheets.RefreshAll();

            // Ottieni il primo slicer nella cartella di lavoro
            var slicer = workbook.Worksheets
                .SelectMany(x => x.Slicers)
                .First();

            // Itera attraverso gli elementi della cache dello slicer
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

### Vedi anche

* namespace [Aspose.Cells.Slicers](../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../)


