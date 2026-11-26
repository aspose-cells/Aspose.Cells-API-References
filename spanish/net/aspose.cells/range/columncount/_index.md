---
title: "Range.ColumnCount"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Range. Obtiene la cantidad de columnas en el rango"
type: docs
url: /es/net/aspose.cells/range/columncount/
---
## Range.ColumnCount property

Obtiene el recuento de columnas en el rango.

```csharp
public int ColumnCount { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangePropertyColumnCountDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet sheet = workbook.Worksheets[0];
            
            // Crear datos de ejemplo (5 columnas x 3 filas)
            for (int col = 0; col < 5; col++)
            {
                for (int row = 0; row < 3; row++)
                {
                    sheet.Cells[row, col].PutValue($"Data {row},{col}");
                }
            }
            
            // Crear un rango que cubra todas las columnas de datos
            Aspose.Cells.Range dataRange = sheet.Cells.CreateRange(0, 0, 3, 5);
            
            // Demostrar el uso de ColumnCount
            Console.WriteLine($"Range has {dataRange.ColumnCount} columns");
            
            // Ajustar automáticamente cada columna en el rango
            for (int i = 0; i < dataRange.ColumnCount; i++)
            {
                sheet.AutoFitColumn(dataRange.FirstColumn + i);
            }
            
            // Guarda el libro de trabajo
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ver también

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


