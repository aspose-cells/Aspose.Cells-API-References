---
title: "Cells.UnhideColumn"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cells-metod. Visar en kolumn igen"
type: docs
url: /sv/net/aspose.cells/cells/unhidecolumn/
---
## Cells.UnhideColumn method

Visar en dold kolumn

```csharp
public void UnhideColumn(int column, double width)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| column | Int32 | Kolumnindex. |
| bredd | Double | Kolumnbredd. |

### Exempel

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
            
            // Dölj kolumn 2
            cells.HideColumn(2);
            
            // Visa kolumn 2 igen med breddjustering (-1 betyder att standardbredd används)
            cells.UnhideColumn(2, -1);
            
            Console.WriteLine("Column 2 width after unhiding: " + cells.Columns[2].Width);
        }
    }
}
```

### Se även

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


