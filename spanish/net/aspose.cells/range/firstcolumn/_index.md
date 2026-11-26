---
title: "Range.FirstColumn"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Range. Obtiene el índice de la primera columna del rango"
type: docs
url: /es/net/aspose.cells/range/firstcolumn/
---
## Range.FirstColumn property

Obtiene el índice de la primera columna del rango.

```csharp
public int FirstColumn { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangePropertyFirstColumnDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crear datos de ejemplo
            worksheet.Cells["A1"].PutValue("Header1");
            worksheet.Cells["B1"].PutValue("Header2");
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["B2"].PutValue(200);

            // Cree un rango
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1", "B2");

            // Demostrar la propiedad FirstColumn
            Console.WriteLine("First column index of range: " + range.FirstColumn);

            // Usar FirstColumn para acceder a las celdas en la primera columna del rango
            for (int i = 0; i < range.RowCount; i++)
            {
                Cell cell = range[i, 0]; // Access first column (index 0) of the range
                Console.WriteLine($"Cell[{i},0] value: {cell.StringValue}");
            }

            // Guarda el libro de trabajo
            workbook.Save("RangeFirstColumnDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


