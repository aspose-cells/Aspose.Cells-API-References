---
title: "CellsHelper.ColumnNameToIndex"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "CellsHelper-Methode. Gibt den Spaltenindex gemäß Spaltennamen zurück"
type: docs
url: /de/net/aspose.cells/cellshelper/columnnametoindex/
---
## CellsHelper.ColumnNameToIndex method

Ermittelt den Spaltenindex anhand des Spaltennamens.

```csharp
public static int ColumnNameToIndex(string columnName)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| columnName | String | Spaltenname. |

### Rückgabewert

Spaltenindex.

### Beispiele

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

### Siehe auch

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


