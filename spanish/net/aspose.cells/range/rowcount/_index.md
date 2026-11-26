---
title: "Range.RowCount"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Range. Obtiene el número de filas en el rango"
type: docs
url: /es/net/aspose.cells/range/rowcount/
---
## Range.RowCount property

Obtiene el recuento de filas en el rango.

```csharp
public int RowCount { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangePropertyRowCountDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Crea datos de muestra en las celdas A1:B10
            for (int row = 0; row < 10; row++)
            {
                for (int col = 0; col < 2; col++)
                {
                    worksheet.Cells[row, col].Value = $"Row{row + 1}Col{col + 1}";
                }
            }

            // Crea un rango con nombre que cubra A1:B10
            worksheet.Cells.CreateRange("A1", "B10").Name = "testRange";
            
            // Obtener el rango nombrado
            Aspose.Cells.Range range = workbook.Worksheets.GetRangeByName("testRange");
            
            // Demostrar la propiedad RowCount
            Console.WriteLine($"Range starts at row: {range.FirstRow}");
            Console.WriteLine($"Range row count: {range.RowCount}");
            Console.WriteLine($"Range starts at column: {range.FirstColumn}");
            Console.WriteLine($"Range column count: {range.ColumnCount}");
        }
    }
}
```

### Ver también

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


