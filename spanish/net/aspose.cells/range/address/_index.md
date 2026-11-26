---
title: "Range.Address"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Range. Obtiene la dirección del rango"
type: docs
url: /es/net/aspose.cells/range/address/
---
## Range.Address property

Obtiene la dirección del rango.

```csharp
public string Address { get; }
```

### Ejemplos

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

            // Crea un rango y demuestra la propiedad Address
            Aspose.Cells.Range range = cells.CreateRange("A1");
            Console.WriteLine("Original range address: " + range.Address);

            // Demuestra GetOffset con Address
            Aspose.Cells.Range offsetRange = range.GetOffset(1, 1);
            Console.WriteLine("Offset range address: " + offsetRange.Address);

            // Demuestra la dirección EntireRow
            Aspose.Cells.Range entireRow = range.EntireRow;
            Console.WriteLine("Entire row address: " + entireRow.Address);

            // Demuestra la dirección EntireColumn
            Aspose.Cells.Range entireColumn = range.EntireColumn;
            Console.WriteLine("Entire column address: " + entireColumn.Address);
        }
    }
}
```

### Ver también

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


