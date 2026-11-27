---
title: "Range.RowHeight"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Range-egenskap. Anger eller hämtar höjden på rader i detta område"
type: docs
url: /sv/net/aspose.cells/range/rowheight/
---
## Range.RowHeight property

Anger eller hämtar höjden på raderna i detta område

```csharp
public double RowHeight { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangePropertyRowHeightDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Sätt in några data i den första raden
            worksheet.Cells["A1"].PutValue("This is a test");
            worksheet.Cells["B1"].PutValue("to demonstrate");
            worksheet.Cells["C1"].PutValue("RowHeight property");

            // Hämta initial radhöjd
            double initialHeight = worksheet.Cells.CreateRange("1:1").RowHeight;
            Console.WriteLine("Initial row height: " + initialHeight);

            // Autoanpassa raden
            worksheet.AutoFitRow(0);

            // Hämta den nya radhöjden efter autoanpassning
            double newHeight = worksheet.Cells.CreateRange("1:1").RowHeight;
            Console.WriteLine("Row height after auto-fit: " + newHeight);

            // Ställ in en ny radhöjd manuellt
            worksheet.Cells.CreateRange("1:1").RowHeight = 30;
            Console.WriteLine("Row height after manual set: " + worksheet.Cells.CreateRange("1:1").RowHeight);
        }
    }
}
```

### Se även

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


