---
title: "Cells.HideRows"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cells-metod. Döljer flera rader"
type: docs
url: /sv/net/aspose.cells/cells/hiderows/
---
## Cells.HideRows method

Döljer flera rader.

```csharp
public void HideRows(int row, int totalRows)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| row | Int32 | Radindexet. |
| totalRows | Int32 | Radnumret. |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodHideRowsWithInt32Int32Demo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fyll i lite data
            for (int i = 0; i < 10; i++)
            {
                for (int j = 0; j < 5; j++)
                {
                    worksheet.Cells[i, j].Value = $"Row {i+1}, Col {j+1}";
                }
            }

            // Dölj rader 3 till 5 (nollbaserat index: 2 till 4)
            worksheet.Cells.HideRows(2, 3);

            // Spara arbetsboken
            workbook.Save("HideRowsExample.xlsx");
        }
    }
}
```

### Se även

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


