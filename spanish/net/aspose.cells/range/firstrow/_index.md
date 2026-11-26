---
title: "Range.FirstRow"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Range. Obtiene el índice de la primera fila del rango"
type: docs
url: /es/net/aspose.cells/range/firstrow/
---
## Range.FirstRow property

Obtiene el índice de la primera fila del rango.

```csharp
public int FirstRow { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangePropertyFirstRowDemo
    {
        public static void Run()
        {
            // Cree un libro de trabajo y acceda a la primera hoja
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Poblar algunos datos
            worksheet.Cells["A1"].PutValue("Header");
            worksheet.Cells["A2"].PutValue("Data1");
            worksheet.Cells["A3"].PutValue("Data2");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);

            // Cree un rango
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1:B3");

            // Acceda y muestre la propiedad FirstRow
            Console.WriteLine("First row index of range: " + range.FirstRow);

            // Acceda a la primera celda de la primera fila del rango
            Cell firstCell = worksheet.Cells[range.FirstRow, range.FirstColumn];
            Console.WriteLine("First cell value: " + firstCell.StringValue);
        }
    }
}
```

### Ver también

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


