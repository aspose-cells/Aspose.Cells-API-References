---
title: "Cells.UnhideRows"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cells-metoden. Visar de dolda raderna"
type: docs
url: /sv/net/aspose.cells/cells/unhiderows/
---
## Cells.UnhideRows method

Visar de dolda raderna.

```csharp
public void UnhideRows(int row, int totalRows, double height)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| row | Int32 | Radindexet. |
| totalRows | Int32 | Radnumret. |
| höjd | Double | Radhöjd. Radvärdet ändras endast när raden är dold och det angivna höjdvärdet är positivt. |

### Exempel

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
            
            // Dölj raderna 0-4
            cells.HideRows(0, 5);
            
            // Visa raderna 0-4 med höjdanpassning (-1 för automatisk anpassning)
            cells.UnhideRows(0, 5, -1);
            
            // Verifiera att raderna är synliga
            for (int i = 0; i < 5; i++)
            {
                Console.WriteLine($"Row {i} hidden status: {cells.IsRowHidden(i)}");
            }
        }
    }
}
```

### Se även

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


