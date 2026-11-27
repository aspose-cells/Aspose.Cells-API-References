---
title: "Range.FirstRow"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Range-egenskap. Hämtar indexet för den första raden i range"
type: docs
url: /sv/net/aspose.cells/range/firstrow/
---
## Range.FirstRow property

Hämtar indexet för den första raden i området.

```csharp
public int FirstRow { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangePropertyFirstRowDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok och öppna första worksheet
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fyll i lite data
            worksheet.Cells["A1"].PutValue("Header");
            worksheet.Cells["A2"].PutValue("Data1");
            worksheet.Cells["A3"].PutValue("Data2");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);

            // Skapa ett intervall
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1:B3");

            // Öppna och visa FirstRow-egenskap
            Console.WriteLine("First row index of range: " + range.FirstRow);

            // Öppna den första cellen i den första raden i range
            Cell firstCell = worksheet.Cells[range.FirstRow, range.FirstColumn];
            Console.WriteLine("First cell value: " + firstCell.StringValue);
        }
    }
}
```

### Se även

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


