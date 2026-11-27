---
title: "Cells.HideColumn"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cells-metod. Döljer en kolumn"
type: docs
url: /sv/net/aspose.cells/cells/hidecolumn/
---
## Cells.HideColumn method

Döljer en kolumn.

```csharp
public void HideColumn(int column)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| column | Int32 | Kolumnindex. |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodHideColumnWithInt32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Sätt in data i kolumnen som vi ska dölja
            cells["B1"].PutValue("This column will be hidden");
            cells["B2"].PutValue(123.45);

            // Dölj kolumn B (index 1)
            cells.HideColumn(1);

            // Ta bort dold status för kolumnen med standardbredd
            cells.UnhideColumn(1, cells.StandardWidth);

            // Spara arbetsboken
            workbook.Save("HideColumnDemo.xlsx");
        }
    }
}
```

### Se även

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


