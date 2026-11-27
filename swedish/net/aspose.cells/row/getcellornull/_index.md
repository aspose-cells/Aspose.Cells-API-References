---
title: "Row.GetCellOrNull"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Row-metod. Hämtar cellen eller null på det specifika indexet"
type: docs
url: /sv/net/aspose.cells/row/getcellornull/
---
## Row.GetCellOrNull method

Hämtar cellen eller null på det specifika indexet.

```csharp
public Cell GetCellOrNull(int column)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| column | Int32 | Kolumnindexet |

### Returvärde

Returnerar cellobjektet om cellen finns. Eller returnerar null om cellobjektet inte finns.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RowMethodGetCellOrNullWithInt32Demo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook wb = new Workbook();
            Worksheet ws = wb.Worksheets[0];

            // Lägg till exempeldata
            ws.Cells["A1"].PutValue("Header1");
            ws.Cells["B1"].PutValue("Header2");
            ws.Cells["A2"].PutValue(100);
            ws.Cells["B2"].PutValue(200);

            // Hämta den första raden
            Row row = ws.Cells.Rows[0];

            // Demonstrera GetCellOrNull med Int32-parameter
            for (int colIndex = 0; colIndex < 2; colIndex++)
            {
                Cell cell = row.GetCellOrNull(colIndex);
                if (cell != null)
                {
                    Console.WriteLine($"Cell at column {colIndex}: {cell.StringValue}");
                }
                else
                {
                    Console.WriteLine($"Cell at column {colIndex} is null");
                }
            }
        }
    }
}
```

### Se även

* class [Cell](../../cell/)
* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


