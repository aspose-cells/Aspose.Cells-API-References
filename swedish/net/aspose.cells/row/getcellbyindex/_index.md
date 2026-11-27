---
title: "Row.GetCellByIndex"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Row-metod. Hämta cellen med ett specifikt index i cellsamlingen för den här raden"
type: docs
url: /sv/net/aspose.cells/row/getcellbyindex/
---
## Row.GetCellByIndex method

Hämta cellen med ett specifikt index i cellsamlingen för den här raden.

```csharp
public Cell GetCellByIndex(int index)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| index | Int32 | Indexet (positionen) för cellen i cellsamlingen för den här raden. |

### Returvärde

Cell-objektet på given position.

### Anmärkningar

För att gå igenom alla celler i sekvens utan modifiering, ger användning av [`GetEnumerator`](../getenumerator/) bättre prestanda än att använda den här metoden för att hämta cellen en i taget.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RowMethodGetCellByIndexWithInt32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till data i cellerna i den första raden
            worksheet.Cells["A1"].PutValue("Cell A1");
            worksheet.Cells["B1"].PutValue("Cell B1");
            worksheet.Cells["C1"].PutValue("Cell C1");

            // Hämta första raden
            Row row = worksheet.Cells.Rows[0];

            // Demonstrera GetCellByIndex med Int32-parameter
            Cell cellAtIndex0 = row.GetCellByIndex(0);
            Cell cellAtIndex1 = row.GetCellByIndex(1);
            Cell cellAtIndex2 = row.GetCellByIndex(2);

            Console.WriteLine("Cell at index 0: " + cellAtIndex0.StringValue);
            Console.WriteLine("Cell at index 1: " + cellAtIndex1.StringValue);
            Console.WriteLine("Cell at index 2: " + cellAtIndex2.StringValue);

            workbook.Save("RowGetCellByIndexDemo.xlsx");
        }
    }
}
```

### Se även

* class [Cell](../../cell/)
* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


