---
title: "CellsHelper.ColumnNameToIndex"
second_title: "Aspose.Cells för .NET API‑referens"
description: "CellsHelper-metod. Hämtar kolumnindex enligt kolumnnamn"
type: docs
url: /sv/net/aspose.cells/cellshelper/columnnametoindex/
---
## CellsHelper.ColumnNameToIndex method

Hämtar kolumnindex enligt kolumnnamn.

```csharp
public static int ColumnNameToIndex(string columnName)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| columnName | String | Kolumnnamn. |

### Returvärde

Kolumnindex.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsHelperMethodColumnNameToIndexWithStringDemo
    {
        public static void Run()
        {
            int columnIndex = CellsHelper.ColumnNameToIndex("BAA");
            string columnName = CellsHelper.ColumnIndexToName(columnIndex);
            
            Console.WriteLine("Column Name: " + columnName);
            Console.WriteLine("Column Index: " + columnIndex);
        }
    }
}
```

### Se även

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


