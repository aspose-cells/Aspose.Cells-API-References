---
title: "Cells.MinDataRow"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Cells. Índice de fila mínimo de la celda que contiene datos"
type: docs
url: /es/net/aspose.cells/cells/mindatarow/
---
## Cells.MinDataRow property

Índice de fila mínimo de la celda que contiene datos.

```csharp
public int MinDataRow { get; }
```

### Observaciones

Devuelve -1 si no hay ninguna celda que contenga datos. Esta propiedad necesita iterar y comprobar celdas y filas de forma dinámica, por lo que es un proceso que consume tiempo y no debe invocarse repetidamente, como usarla directamente como condición en un bucle.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyMinDataRowDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Poblar algunos datos
            sheet.Cells[0, 0].Value = "Header1";
            sheet.Cells[0, 1].Value = "Header2";
            sheet.Cells[1, 0].Value = "Data1";
            sheet.Cells[1, 1].Value = "Data2";
            sheet.Cells[2, 0].Value = "Data3";
            sheet.Cells[2, 1].Value = "Data4";

            // Demostrar el uso de MinDataRow
            Console.WriteLine("Minimum data row index: " + sheet.Cells.MinDataRow);
            Console.WriteLine("Maximum data row index: " + sheet.Cells.MaxDataRow);

            // Guarda el libro de trabajo
            workbook.Save("MinDataRowExample.xlsx");
        }
    }
}
```

### Ver también

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


