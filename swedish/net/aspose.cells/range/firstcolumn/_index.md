---
title: "Range.FirstColumn"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Range‑egenskap. Hämtar indexet för den första kolumnen i området"
type: docs
url: /sv/net/aspose.cells/range/firstcolumn/
---
## Range.FirstColumn property

Hämtar indexet för den första kolumnen i området.

```csharp
public int FirstColumn { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangePropertyFirstColumnDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa exempeldata
            worksheet.Cells["A1"].PutValue("Header1");
            worksheet.Cells["B1"].PutValue("Header2");
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["B2"].PutValue(200);

            // Skapa ett intervall
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1", "B2");

            // Demonstrera FirstColumn‑egenskapen
            Console.WriteLine("First column index of range: " + range.FirstColumn);

            // Använd FirstColumn för att komma åt celler i den första kolumnen i området
            for (int i = 0; i < range.RowCount; i++)
            {
                Cell cell = range[i, 0]; // Access first column (index 0) of the range
                Console.WriteLine($"Cell[{i},0] value: {cell.StringValue}");
            }

            // Spara arbetsboken
            workbook.Save("RangeFirstColumnDemo.xlsx");
        }
    }
}
```

### Se även

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


