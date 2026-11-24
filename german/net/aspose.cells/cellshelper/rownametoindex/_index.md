---
title: "CellsHelper.RowNameToIndex"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "CellsHelper-Methode. Gibt den Zeilenindex basierend auf dem Zeilennamen zurück"
type: docs
url: /de/net/aspose.cells/cellshelper/rownametoindex/
---
## CellsHelper.RowNameToIndex method

Ermittelt den Zeilenindex anhand des Zeilennamens.

```csharp
public static int RowNameToIndex(string rowName)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| rowName | String | Zeilenname. |

### Rückgabewert

Zeilenindex.

### Beispiele

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

### Siehe auch

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


