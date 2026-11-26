---
title: "Row.LastCell"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Row. Obtiene el objeto de la última celda en la fila"
type: docs
url: /es/net/aspose.cells/row/lastcell/
---
## Row.LastCell property

Obtiene el último objeto de celda en la fila.

```csharp
public Cell LastCell { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RowPropertyLastCellDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de muestra a las celdas
            worksheet.Cells["A1"].PutValue("First");
            worksheet.Cells["B1"].PutValue("Second");
            worksheet.Cells["C1"].PutValue("Last");

            // Obtener la primera fila
            Row row = worksheet.Cells.Rows[0];

            // Acceder a la última celda en la fila
            Cell lastCell = row.LastCell;
            
            // Mostrar el valor de la última celda
            Console.WriteLine("Last cell value: " + lastCell.Value);
        }
    }
}
```

### Ver también

* class [Cell](../../cell/)
* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


