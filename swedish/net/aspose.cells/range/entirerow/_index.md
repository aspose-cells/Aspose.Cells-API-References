---
title: "Range.EntireRow"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Range-egenskapen. Hämtar ett Range‑objekt som representerar hela raden eller raderna som innehåller det angivna området"
type: docs
url: /sv/net/aspose.cells/range/entirerow/
---
## Range.EntireRow property

Hämtar ett Range-objekt som representerar hela raden (eller raderna) som innehåller det angivna området.

```csharp
public Range EntireRow { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangePropertyEntireRowDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Fyll i lite exempeldata i den första raden
            for (int col = 0; col < 5; col++)
            {
                sheet.Cells[0, col].PutValue($"Header {col + 1}");
            }

            // Hämta hela den första raden med EntireRow‑egenskapen
            Aspose.Cells.Range entireRow = sheet.Cells.CreateRange("A1").EntireRow;

            // Kopiera den första raden till den tredje raden
            Aspose.Cells.Range destination = sheet.Cells.CreateRange("A3").EntireRow;
            destination.Copy(entireRow);

            // Spara arbetsboken
            workbook.Save("EntireRowDemo.xlsx");
        }
    }
}
```

### Se även

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


