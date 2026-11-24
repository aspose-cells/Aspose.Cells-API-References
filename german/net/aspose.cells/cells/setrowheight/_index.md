---
title: "Cells.SetRowHeight"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cells-Methode. Legt die Höhe der angegebenen Zeile fest"
type: docs
url: /de/net/aspose.cells/cells/setrowheight/
---
## Cells.SetRowHeight method

Setzt die Höhe der angegebenen Zeile.

```csharp
public void SetRowHeight(int row, double height)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| row | Int32 | Zeilenindex. |
| Höhe | Double | Höhe der Zeile. In Punkt angegeben. Sie sollte zwischen 0 und 409,5 liegen. |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodSetRowHeightWithInt32DoubleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Setze die Zeilenhöhe für die erste Zeile (Index 0) auf 25,5 Punkte
            cells.SetRowHeight(0, 25.5);

            // Überprüfe die Zeilenhöhe
            Console.WriteLine("Row height of row 0: " + cells.GetRowHeight(0));
        }
    }
}
```

### Siehe auch

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


