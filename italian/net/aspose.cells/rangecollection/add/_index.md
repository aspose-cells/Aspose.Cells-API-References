---
title: "RangeCollection.Add"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo RangeCollection. Aggiunge un elemento Range alla collezione"
type: docs
url: /it/net/aspose.cells/rangecollection/add/
---
## RangeCollection.Add method

Aggiunge un elemento [`Range`](../../range/) alla collezione.

```csharp
[Obsolete("Use RangeCollection.AddRange(Range) method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int Add(Range range)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| intervallo | Intervallo | Oggetto Range |

### Osservazioni

NOTA: Questo membro è ora obsoleto. Invece, si prega di utilizzare il metodo AddRange(). Questo metodo sarà rimosso 6 mesi dopo, a partire da dicembre 2025. Aspose si scusa per qualsiasi inconveniente tu possa aver riscontrato.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangeCollectionMethodAddWithRangeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Crea un range e aggiungilo alla collezione
            Aspose.Cells.Range cellRange = worksheet.Cells.CreateRange(0, 0, 3, 1);
            worksheet.Cells.Ranges.Add(cellRange);
            
            // Inserisci righe per dimostrare l'espansione del range
            worksheet.Cells.InsertRows(2, 2);
            
            Console.WriteLine("Range row count after insertion: " + cellRange.RowCount);
        }
    }
}
```

### Vedi anche

* class [Range](../../range/)
* class [RangeCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


