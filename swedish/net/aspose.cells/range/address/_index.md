---
title: "Range.Address"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Range‑egenskap. Hämtar adressen för området"
type: docs
url: /sv/net/aspose.cells/range/address/
---
## Range.Address property

Hämtar adressen för området.

```csharp
public string Address { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangePropertyAddressDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Skapa ett område och demonstrera Address‑egenskapen
            Aspose.Cells.Range range = cells.CreateRange("A1");
            Console.WriteLine("Original range address: " + range.Address);

            // Demonstrera GetOffset med Address
            Aspose.Cells.Range offsetRange = range.GetOffset(1, 1);
            Console.WriteLine("Offset range address: " + offsetRange.Address);

            // Demonstrera EntireRow‑adress
            Aspose.Cells.Range entireRow = range.EntireRow;
            Console.WriteLine("Entire row address: " + entireRow.Address);

            // Demonstrera EntireColumn‑adress
            Aspose.Cells.Range entireColumn = range.EntireColumn;
            Console.WriteLine("Entire column address: " + entireColumn.Address);
        }
    }
}
```

### Se även

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


