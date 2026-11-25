---
title: "Range.Address"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Range. Ottiene l'indirizzo dell'intervallo"
type: docs
url: /it/net/aspose.cells/range/address/
---
## Range.Address property

Ottiene l'indirizzo dell'intervallo.

```csharp
public string Address { get; }
```

### Esempi

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

            // Crea un intervallo e dimostra la proprietà Address
            Aspose.Cells.Range range = cells.CreateRange("A1");
            Console.WriteLine("Original range address: " + range.Address);

            // Dimostra GetOffset con Address
            Aspose.Cells.Range offsetRange = range.GetOffset(1, 1);
            Console.WriteLine("Offset range address: " + offsetRange.Address);

            // Dimostra l'indirizzo EntireRow
            Aspose.Cells.Range entireRow = range.EntireRow;
            Console.WriteLine("Entire row address: " + entireRow.Address);

            // Dimostra l'indirizzo EntireColumn
            Aspose.Cells.Range entireColumn = range.EntireColumn;
            Console.WriteLine("Entire column address: " + entireColumn.Address);
        }
    }
}
```

### Vedi anche

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


