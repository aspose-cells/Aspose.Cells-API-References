---
title: "Cells.UnhideRows"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cells-Methode. Blendet die versteckten Zeilen ein"
type: docs
url: /de/net/aspose.cells/cells/unhiderows/
---
## Cells.UnhideRows method

Blendet die ausgeblendeten Zeilen ein.

```csharp
public void UnhideRows(int row, int totalRows, double height)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| row | Int32 | Der Zeilenindex. |
| totalRows | Int32 | Die Zeilennummer. |
| Höhe | Double | Zeilenhöhe. Die Höhe der Zeile wird nur geändert, wenn die Zeile ausgeblendet ist und der angegebene Höhenwert positiv ist. |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodUnhideRowsWithInt32Int32DoubleDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Cells cells = wb.Worksheets[0].Cells;
            
            // Verstecke Zeilen 0-4
            cells.HideRows(0, 5);
            
            // Blende Zeilen 0-4 mit Höhenanpassung ein (-1 für automatische Anpassung)
            cells.UnhideRows(0, 5, -1);
            
            // Überprüfe, ob die Zeilen eingeblendet sind
            for (int i = 0; i < 5; i++)
            {
                Console.WriteLine($"Row {i} hidden status: {cells.IsRowHidden(i)}");
            }
        }
    }
}
```

### Siehe auch

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


