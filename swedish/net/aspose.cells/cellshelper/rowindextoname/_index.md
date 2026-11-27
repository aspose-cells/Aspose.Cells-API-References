---
title: "CellsHelper.RowIndexToName"
second_title: "Aspose.Cells för .NET API‑referens"
description: "CellsHelper-metod. Hämtar radnamn enligt radindex"
type: docs
url: /sv/net/aspose.cells/cellshelper/rowindextoname/
---
## CellsHelper.RowIndexToName method

Hämtar radnamn enligt radindex.

```csharp
public static string RowIndexToName(int row)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| row | Int32 | Radindex. |

### Returvärde

Radens namn.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsHelperMethodRowIndexToNameWithInt32Demo
    {
        public static void Run()
        {
            int rowIndex = 10;
            string rowName = CellsHelper.RowIndexToName(rowIndex);
            Console.WriteLine("Row index {0} corresponds to row name: {1}", rowIndex, rowName);
            
            int convertedBackIndex = CellsHelper.RowNameToIndex(rowName);
            Console.WriteLine("Row name {0} converted back to index: {1}", rowName, convertedBackIndex);
        }
    }
}
```

### Se även

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


