---
title: "WorksheetCollection.CreateRange"
second_title: "Aspose.Cells för .NET API‑referens"
description: "WorksheetCollection-metod. Skapar ett Range-objekt från en adress för intervallet."
type: docs
url: /sv/net/aspose.cells/worksheetcollection/createrange/
---
## WorksheetCollection.CreateRange method

Skapar ett [`Range`](../../range/) objekt från en adress för intervallet.

```csharp
public Range CreateRange(string address, int sheetIndex)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| adress | String | Adressen för intervallet. |
| sheetIndex | Int32 | Bladindexet. |

### Returvärde

Ett [`Range`](../../range/) objekt

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionMethodCreateRangeWithStringInt32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fyll i lite exempeldata
            for (int i = 0; i < 10; i++)
            {
                for (int j = 0; j < 6; j++)
                {
                    worksheet.Cells[i, j].PutValue($"Cell {i+1},{j+1}");
                }
            }

            // Skapa intervall med strängadress och bladindex
            Aspose.Cells.Range range = workbook.Worksheets.CreateRange("A1:F10", 0);

            // Demonstrera användning av intervall
            Console.WriteLine($"Range has {range.RowCount} rows and {range.ColumnCount} columns");
            Console.WriteLine($"First cell value: {range[0, 0].StringValue}");
            Console.WriteLine($"Last cell value: {range[9, 5].StringValue}");
        }
    }
}
```

### Se även

* class [Range](../../range/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


