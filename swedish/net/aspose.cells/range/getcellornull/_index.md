---
title: "Range.GetCellOrNull"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Range‑metod. Hämtar Cell‑objekt eller null i detta intervall"
type: docs
url: /sv/net/aspose.cells/range/getcellornull/
---
## Range.GetCellOrNull method

Hämtar [`Cell`](../../cell/) objekt eller null i detta intervall.

```csharp
public Cell GetCellOrNull(int rowOffset, int columnOffset)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rowOffset | Int32 | Radoffset i detta intervall, nollbaserat. |
| columnOffset | Int32 | Kolumnoffset i detta intervall, nollbaserat. |

### Returvärde

[`Cell`](../../cell/) object.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangeMethodGetCellOrNullWithInt32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa ett intervall
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1:B2");
            
            // Fyll i några data i intervallet
            range[0, 0].PutValue("Cell A1");
            range[0, 1].PutValue("Cell B1");
            range[1, 0].PutValue("Cell A2");
            
            // Demonstrera GetCellOrNull med Int32‑parametrar
            Cell cell1 = range.GetCellOrNull(0, 0);
            Console.WriteLine("Cell (0,0): " + (cell1 != null ? cell1.StringValue : "null"));
            
            Cell cell2 = range.GetCellOrNull(1, 1);
            Console.WriteLine("Cell (1,1): " + (cell2 != null ? cell2.StringValue : "null"));
            
            // Försök att hämta en cell utanför intervallet (ska returnera null)
            Cell cell3 = range.GetCellOrNull(2, 0);
            Console.WriteLine("Cell (2,0): " + (cell3 != null ? cell3.StringValue : "null"));
        }
    }
}
```

### Se även

* class [Cell](../../cell/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


