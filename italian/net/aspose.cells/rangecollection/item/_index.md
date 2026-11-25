---
title: "RangeCollection.Item"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà RangeCollection. Ottiene l'elemento Range all'indice specificato"
type: docs
url: /it/net/aspose.cells/rangecollection/item/
---
## RangeCollection indexer

Ottiene l'elemento [`Range`](../../range/) all'indice specificato.

```csharp
public Range this[int index] { get; }
```

| Parametro | Descrizione |
| --- | --- |
| indice | L'indice a base zero dell'elemento. |

### Valore di ritorno

L'elemento all'indice specificato.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangeCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea alcuni intervalli
            Aspose.Cells.Range range1 = worksheet.Cells.CreateRange("A1:B2");
            Aspose.Cells.Range range2 = worksheet.Cells.CreateRange("C3:D4");
            Aspose.Cells.Range range3 = worksheet.Cells.CreateRange("E5:F6");

            // Aggiungi intervalli alla collezione
            RangeCollection ranges = worksheet.Cells.Ranges;
            ranges.Add(range1);
            ranges.Add(range2);
            ranges.Add(range3);

            // Dimostra l'uso della proprietà Item
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

            // Accedi a un intervallo specifico per indice
            Aspose.Cells.Range secondRange = ranges[1]; // Using Item property
            Console.WriteLine("\nSecond range details:");
            Console.WriteLine($"Address: {secondRange.Address}");
        }
    }
}
```

### Vedi anche

* class [Range](../../range/)
* class [RangeCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


