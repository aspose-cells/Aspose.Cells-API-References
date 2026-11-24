---
title: "Cells.UnhideColumn"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cells-Methode. Blendet eine Spalte ein"
type: docs
url: /de/net/aspose.cells/cells/unhidecolumn/
---
## Cells.UnhideColumn method

Blendet eine Spalte ein

```csharp
public void UnhideColumn(int column, double width)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| column | Int32 | Spaltenindex. |
| Breite | Double | Spaltenbreite. |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodUnhideColumnWithInt32DoubleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            
            // Spalte 2 ausblenden
            cells.HideColumn(2);
            
            // Spalte 2 einblenden mit Breitenanpassung (-1 bedeutet Standardbreite verwenden)
            cells.UnhideColumn(2, -1);
            
            Console.WriteLine("Column 2 width after unhiding: " + cells.Columns[2].Width);
        }
    }
}
```

### Siehe auch

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


