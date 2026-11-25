---
title: "CellArea.CompareTo"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo CellArea. Confronta due oggetti CellArea secondo il loro angolo in alto a sinistra"
type: docs
url: /it/net/aspose.cells/cellarea/compareto/
---
## CellArea.CompareTo method

Confronta due oggetti CellArea in base al loro angolo in alto a sinistra.

```csharp
public int CompareTo(object obj)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| obj | Object |  |

### Valore di ritorno

Se due angoli sono in righe diverse, confronta il loro indice di riga. Altrimenti confronta il loro indice di colonna. Se i due angoli sono uguali, verrà restituito 0.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellAreaMethodCompareToWithObjectDemo
    {
        public static void Run()
        {
            // Crea due oggetti CellArea per il confronto
            CellArea ca1 = new CellArea { StartRow = 0, EndRow = 10, StartColumn = 0, EndColumn = 10 };
            object ca2 = new CellArea { StartRow = 0, EndRow = 5, StartColumn = 0, EndColumn = 5 };

            // Dimostra il metodo CompareTo con parametro Object
            int comparisonResult = ca1.CompareTo(ca2);
            Console.WriteLine($"Comparison result: {comparisonResult}");

            // Crea un altro confronto con aree uguali
            object ca3 = new CellArea { StartRow = 0, EndRow = 10, StartColumn = 0, EndColumn = 10 };
            comparisonResult = ca1.CompareTo(ca3);
            Console.WriteLine($"Comparison result with equal areas: {comparisonResult}");
        }
    }
}
```

### Vedi anche

* struct [CellArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


