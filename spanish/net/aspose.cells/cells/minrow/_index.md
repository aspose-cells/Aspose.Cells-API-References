---
title: "Cells.MinRow"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Cells. Índice de fila mínimo de la celda que contiene datos o estilo"
type: docs
url: /es/net/aspose.cells/cells/minrow/
---
## Cells.MinRow property

Índice de fila mínimo de la celda que contiene datos o estilo.

```csharp
public int MinRow { get; }
```

### Observaciones

Esta propiedad necesita iterar y comprobar celdas y filas de forma dinámica, por lo que es un proceso que consume tiempo y no debe invocarse repetidamente, como usarla directamente como condición en un bucle.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyMinRowDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Agregar algunos datos para demostrar MinRow
            cells["A1"].PutValue("Data in first row");
            cells["B5"].PutValue("Data in fifth row");

            // Mostrar información de MinRow
            Console.WriteLine("Minimum used row: " + cells.MinRow);
            Console.WriteLine("Maximum used row: " + cells.MaxRow);

            // Borrar el contenido a partir de MinRow
            cells.ClearContents(cells.MinRow, cells.MinColumn, cells.MaxRow, cells.MaxColumn);

            // Verificar la eliminación comprobando si las celdas están vacías
            Console.WriteLine("A1 after clearing: " + (cells["A1"].Value == null ? "Empty" : "Not empty"));
            Console.WriteLine("B5 after clearing: " + (cells["B5"].Value == null ? "Empty" : "Not empty"));
        }
    }
}
```

### Ver también

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


