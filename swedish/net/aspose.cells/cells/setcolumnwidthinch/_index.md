---
title: "Cells.SetColumnWidthInch"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cells-metod. Ställer in kolumnbredd i enheten tum i normal vy"
type: docs
url: /sv/net/aspose.cells/cells/setcolumnwidthinch/
---
## Cells.SetColumnWidthInch method

Ställer in kolumnbredd i tum i normal vy.

```csharp
public void SetColumnWidthInch(int column, double inches)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| column | Int32 | Kolumnindex. |
| tum | Double | Antal tum. |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodSetColumnWidthInchWithInt32DoubleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Ställ in kolumnbredder i tum
            cells.SetColumnWidthInch(0, 2.0);
            cells.SetColumnWidthInch(1, 1.5);
            cells.SetColumnWidthInch(2, 0.8);

            // Sätt in lite data i celler för att göra filen synlig
            cells["A1"].PutValue("Column A (2 inches)");
            cells["B1"].PutValue("Column B (1.5 inches)");
            cells["C1"].PutValue("Column C (0.8 inches)");

            // Spara arbetsboken
            workbook.Save("ColumnWidthsInInches.xlsx");
        }
    }
}
```

### Se även

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


