---
title: "Cells.MoveRange"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cells-metod. Flyttar området"
type: docs
url: /sv/net/aspose.cells/cells/moverange/
---
## Cells.MoveRange method

Flyttar området.

```csharp
public void MoveRange(CellArea sourceArea, int destRow, int destColumn)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sourceArea | CellArea | Området som ska flyttas. |
| destRow | Int32 | Målraden. |
| destColumn | Int32 | Målkolumnen. |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodMoveRangeWithCellAreaInt32Int32Demo
    {
        public static void Run()
        {
            // Skapa en arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Sätt värden i celler
            cells["A1"].PutValue("Original");
            cells["B1"].PutValue(100);
            cells["A2"].PutValue("Data");
            cells["B2"].PutValue(200);

            // Definiera cellområdet som ska flyttas (A1:B2)
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 1;
            area.EndColumn = 1;

            // Flytta området neråt med 2 rader och åt höger med 3 kolumner
            cells.MoveRange(area, 2, 3);

            // Spara arbetsboken
            workbook.Save("MoveRangeExample.xlsx");
        }
    }
}
```

### Se även

* struct [CellArea](../../cellarea/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


