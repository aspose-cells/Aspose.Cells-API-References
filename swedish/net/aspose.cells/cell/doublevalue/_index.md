---
title: "Cell.DoubleValue"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cell-egenskap. Hämtar det dubbelvärde som finns i cellen"
type: docs
url: /sv/net/aspose.cells/cell/doublevalue/
---
## Cell.DoubleValue property

Hämtar dubbelvärdet som finns i cellen.

```csharp
public double DoubleValue { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyDoubleValueDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Ställ in olika värdetyper i celler
            cells["A1"].PutValue(1); // Int value
            cells["A2"].PutValue(true); // Bool value
            cells["A3"].PutValue("abc"); // String value
            cells["A4"].PutValue(false); // Bool value
            cells["A5"].PutValue(2.56); // Double value

            // Demonstrera DoubleValue-egenskapen
            Console.WriteLine("Double value from cell A5: " + cells["A5"].DoubleValue);
            
            // Verifiera att andra värdetyper kan läsas som dubbel
            Console.WriteLine("Int as double from A1: " + cells["A1"].DoubleValue);
            Console.WriteLine("Bool as double from A2: " + cells["A2"].DoubleValue);
        }
    }
}
```

### Se även

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


