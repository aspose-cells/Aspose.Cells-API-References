---
title: "Range.GetOffset"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Range‑metod. Hämtar Range‑område med förskjutning"
type: docs
url: /sv/net/aspose.cells/range/getoffset/
---
## Range.GetOffset method

Hämtar [`Range`](../) område med förskjutning.

```csharp
public Range GetOffset(int rowOffset, int columnOffset)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rowOffset | Int32 | Radoffset i detta intervall, nollbaserat. |
| columnOffset | Int32 | Kolumnoffset i detta intervall, nollbaserat. |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangeMethodGetOffsetWithInt32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;
            
            // Skapa initialt område
            Aspose.Cells.Range originalRange = cells.CreateRange("A1");
            Console.WriteLine("Original Range Address: " + originalRange.Address);
            
            // Hämta förskjutningsområde
            Aspose.Cells.Range offsetRange = originalRange.GetOffset(1, 1);
            Console.WriteLine("Offset Range Address: " + offsetRange.Address);
        }
    }
}
```

### Se även

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


