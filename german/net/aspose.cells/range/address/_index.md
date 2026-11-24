---
title: "Range.Address"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Range-Eigenschaft. Gibt die Adresse des Bereichs zurück"
type: docs
url: /de/net/aspose.cells/range/address/
---
## Range.Address property

Liefert die Adresse des Bereichs.

```csharp
public string Address { get; }
```

### Beispiele

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

            // Erstellen Sie einen Bereich und demonstrieren Sie die Address-Eigenschaft
            Aspose.Cells.Range range = cells.CreateRange("A1");
            Console.WriteLine("Original range address: " + range.Address);

            // Demonstrieren Sie GetOffset mit Address
            Aspose.Cells.Range offsetRange = range.GetOffset(1, 1);
            Console.WriteLine("Offset range address: " + offsetRange.Address);

            // Demonstrieren Sie die EntireRow-Adresse
            Aspose.Cells.Range entireRow = range.EntireRow;
            Console.WriteLine("Entire row address: " + entireRow.Address);

            // Demonstrieren Sie die EntireColumn-Adresse
            Aspose.Cells.Range entireColumn = range.EntireColumn;
            Console.WriteLine("Entire column address: " + entireColumn.Address);
        }
    }
}
```

### Siehe auch

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


