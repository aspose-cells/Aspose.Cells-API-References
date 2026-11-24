---
title: "CellsHelper.RowIndexToName"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "CellsHelper-Methode. Gibt den Zeilennamen gemäß Zeilenindex zurück"
type: docs
url: /de/net/aspose.cells/cellshelper/rowindextoname/
---
## CellsHelper.RowIndexToName method

Ermittelt den Zeilennamen anhand des Zeilenindex.

```csharp
public static string RowIndexToName(int row)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| row | Int32 | Zeilenindex. |

### Rückgabewert

Name der Zeile.

### Beispiele

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

### Siehe auch

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


