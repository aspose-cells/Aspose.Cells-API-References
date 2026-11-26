---
title: "Cells.MinColumn"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Cells. Índice de columna mínimo de aquellas celdas que se han instanciado en la colección no incluye la columna donde el estilo está definido para toda la columna pero no se ha instanciado ninguna celda en ella"
type: docs
url: /es/net/aspose.cells/cells/mincolumn/
---
## Cells.MinColumn property

Índice mínimo de columna de esas celdas que han sido instanciadas en la colección (no incluye la columna donde el estilo está definido para toda la columna pero no se ha instanciado ninguna celda en ella).

```csharp
public int MinColumn { get; }
```

### Observaciones

Esta propiedad necesita iterar y comprobar celdas y filas de forma dinámica, por lo que es un proceso que consume tiempo y no debe invocarse repetidamente, como usarla directamente como condición en un bucle.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyMinColumnDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Acceder a la colección de celdas
            Cells cells = worksheet.Cells;
            
            // Poblar algunos datos en las columnas 2, 3 y 4 (B, C, D)
            cells["B1"].PutValue("Data in Column B");
            cells["C1"].PutValue("Data in Column C");
            cells["D1"].PutValue("Data in Column D");
            
            // Obtener el índice de columna mínimo que contiene datos
            int minColumn = cells.MinColumn;
            
            // Obtener el índice de columna máximo que contiene datos
            int maxColumn = cells.MaxColumn;
            
            Console.WriteLine("Minimum column with data: " + minColumn); // Should output 1 (column B)
            Console.WriteLine("Maximum column with data: " + maxColumn); // Should output 3 (column D)
            
            // Borrar la columna B para demostrar el cambio de MinColumn
            cells.DeleteColumn(1);
            
            Console.WriteLine("\nAfter deleting column B:");
            Console.WriteLine("New minimum column with data: " + cells.MinColumn); // Should now output 2 (column C)
            Console.WriteLine("Maximum column with data: " + cells.MaxColumn); // Should still output 3 (column D)
        }
    }
}
```

### Ver también

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


