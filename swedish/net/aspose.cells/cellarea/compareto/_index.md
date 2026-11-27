---
title: "CellArea.CompareTo"
second_title: "Aspose.Cells för .NET API‑referens"
description: "CellArea-metod. Jämför två CellArea-objekt enligt deras övre vänstra hörn"
type: docs
url: /sv/net/aspose.cells/cellarea/compareto/
---
## CellArea.CompareTo method

Jämför två CellArea-objekt enligt deras övre vänstra hörn.

```csharp
public int CompareTo(object obj)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| obj | Object |  |

### Returvärde

Om två hörn ligger i olika rader jämförs deras radindex. Annars jämförs deras kolumnindex. Om två hörn är lika returneras 0.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellAreaMethodCompareToWithObjectDemo
    {
        public static void Run()
        {
            // Skapa två CellArea-objekt för jämförelse
            CellArea ca1 = new CellArea { StartRow = 0, EndRow = 10, StartColumn = 0, EndColumn = 10 };
            object ca2 = new CellArea { StartRow = 0, EndRow = 5, StartColumn = 0, EndColumn = 5 };

            // Demonstrera CompareTo-metoden med Object-parameter
            int comparisonResult = ca1.CompareTo(ca2);
            Console.WriteLine($"Comparison result: {comparisonResult}");

            // Skapa en annan jämförelse med lika områden
            object ca3 = new CellArea { StartRow = 0, EndRow = 10, StartColumn = 0, EndColumn = 10 };
            comparisonResult = ca1.CompareTo(ca3);
            Console.WriteLine($"Comparison result with equal areas: {comparisonResult}");
        }
    }
}
```

### Se även

* struct [CellArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


