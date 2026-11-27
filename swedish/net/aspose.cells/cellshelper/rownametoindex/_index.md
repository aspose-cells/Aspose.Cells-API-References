---
title: "CellsHelper.RowNameToIndex"
second_title: "Aspose.Cells för .NET API‑referens"
description: "CellsHelper-metod. Hämtar radindex enligt radnamn"
type: docs
url: /sv/net/aspose.cells/cellshelper/rownametoindex/
---
## CellsHelper.RowNameToIndex method

Hämtar radindex enligt radnamn.

```csharp
public static int RowNameToIndex(string rowName)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rowName | String | Radnamn. |

### Returvärde

Radindex.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsHelperMethodRowNameToIndexWithStringDemo
    {
        public static void Run()
        {
            string rowName = "11";
            int rowIndex = CellsHelper.RowNameToIndex(rowName);
            Console.WriteLine("Row name '{0}' converted to index: {1}", rowName, rowIndex);
        }
    }
}
```

### Se även

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


