---
title: "CellArea.CompareTo"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "CellArea-Methode. Vergleicht zwei CellArea-Objekte anhand ihrer oberen linken Ecke"
type: docs
url: /de/net/aspose.cells/cellarea/compareto/
---
## CellArea.CompareTo method

Vergleicht zwei CellArea-Objekte anhand ihrer oberen linken Ecke.

```csharp
public int CompareTo(object obj)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| obj | Object |  |

### Rückgabewert

Wenn sich die beiden Ecken in unterschiedlichen Zeilen befinden, vergleichen Sie deren Zeilenindex. Andernfalls vergleichen Sie deren Spaltenindex. Wenn die beiden Ecken gleich sind, wird 0 zurückgegeben.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellAreaMethodCompareToWithObjectDemo
    {
        public static void Run()
        {
            // Erstellen Sie zwei CellArea-Objekte zum Vergleich
            CellArea ca1 = new CellArea { StartRow = 0, EndRow = 10, StartColumn = 0, EndColumn = 10 };
            object ca2 = new CellArea { StartRow = 0, EndRow = 5, StartColumn = 0, EndColumn = 5 };

            // Demonstrieren Sie die CompareTo-Methode mit dem Objektparameter
            int comparisonResult = ca1.CompareTo(ca2);
            Console.WriteLine($"Comparison result: {comparisonResult}");

            // Erstellen Sie einen weiteren Vergleich mit gleichen Bereichen
            object ca3 = new CellArea { StartRow = 0, EndRow = 10, StartColumn = 0, EndColumn = 10 };
            comparisonResult = ca1.CompareTo(ca3);
            Console.WriteLine($"Comparison result with equal areas: {comparisonResult}");
        }
    }
}
```

### Siehe auch

* struct [CellArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


