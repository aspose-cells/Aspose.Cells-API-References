---
title: "Cells.MaxRow"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Cells. Índice máximo de fila de la celda que contiene datos o estilo"
type: docs
url: /es/net/aspose.cells/cells/maxrow/
---
## Cells.MaxRow property

Índice máximo de fila de la celda que contiene datos o estilo.

```csharp
public int MaxRow { get; }
```

### Observaciones

Devuelve -1 si no hay ninguna celda que contenga datos o estilo en la hoja de cálculo. Esta propiedad necesita iterar y comprobar celdas y filas de forma dinámica, por lo que es un proceso que consume tiempo y no debe invocarse repetidamente, como usarla directamente como condición en un bucle.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyMaxRowDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Agregar algunos datos de ejemplo
            cells[0, 0].PutValue("Name");
            cells[0, 1].PutValue("Age");
            cells[1, 0].PutValue("John");
            cells[1, 1].PutValue(30);
            cells[2, 0].PutValue("Alice");
            cells[2, 1].PutValue(25);

            // Obtener el índice máximo de fila (basado en cero)
            int maxRow = cells.MaxRow;
            Console.WriteLine("MaxRow before adding new data: " + maxRow);

            // Agregar nuevos datos en la fila siguiente después de la fila máxima
            int newRow = maxRow + 1;
            cells[newRow, 0].PutValue("Bob");
            cells[newRow, 1].PutValue(28);

            // Verificar la nueva fila máxima
            Console.WriteLine("MaxRow after adding new data: " + cells.MaxRow);

            // Guarda el libro de trabajo
            workbook.Save("MaxRowDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


