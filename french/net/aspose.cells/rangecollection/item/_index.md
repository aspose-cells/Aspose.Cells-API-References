---
title: "RangeCollection.Item"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété RangeCollection. Obtient l'élément Range à l'index spécifié"
type: docs
url: /fr/net/aspose.cells/rangecollection/item/
---
## RangeCollection indexer

Obtient l'élément [`Range`](../../range/) à l'index spécifié.

```csharp
public Range this[int index] { get; }
```

| Paramètre | Description |
| --- | --- |
| indice | L'indice à base zéro de l'élément. |

### Valeur de retour

L’élément à l’index spécifié.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangeCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Créer un classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créer quelques plages
            Aspose.Cells.Range range1 = worksheet.Cells.CreateRange("A1:B2");
            Aspose.Cells.Range range2 = worksheet.Cells.CreateRange("C3:D4");
            Aspose.Cells.Range range3 = worksheet.Cells.CreateRange("E5:F6");

            // Ajoutez des plages à la collection
            RangeCollection ranges = worksheet.Cells.Ranges;
            ranges.Add(range1);
            ranges.Add(range2);
            ranges.Add(range3);

            // Démontrer l'utilisation de la propriété Item
            Console.WriteLine("Range Collection Count: " + ranges.Count);
            for (int i = 0; i < ranges.Count; i++)
            {
                Aspose.Cells.Range currentRange = ranges[i]; // Using Item property
                Console.WriteLine($"Range {i + 1}: {currentRange.Address}");
                Console.WriteLine($"  - FirstRow: {currentRange.FirstRow}");
                Console.WriteLine($"  - FirstColumn: {currentRange.FirstColumn}");
                Console.WriteLine($"  - RowCount: {currentRange.RowCount}");
                Console.WriteLine($"  - ColumnCount: {currentRange.ColumnCount}");
            }

            // Accéder à une plage spécifique par index
            Aspose.Cells.Range secondRange = ranges[1]; // Using Item property
            Console.WriteLine("\nSecond range details:");
            Console.WriteLine($"Address: {secondRange.Address}");
        }
    }
}
```

### Voir aussi

* class [Range](../../range/)
* class [RangeCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


