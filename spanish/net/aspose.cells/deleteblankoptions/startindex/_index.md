---
title: "DeleteBlankOptions.StartIndex"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad DeleteBlankOptions. Especifica el índice de fila/columna inicial del rango a comprobar y eliminar filas/columnas en blanco"
type: docs
url: /es/net/aspose.cells/deleteblankoptions/startindex/
---
## DeleteBlankOptions.StartIndex property

Especifica el índice inicial de fila/columna del rango a comprobar y eliminar fila/columna en blanco.

```csharp
public int StartIndex { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DeleteBlankOptionsPropertyStartIndexDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            Cells cells = sheet.Cells;

            // Rellene algunas celdas con valores
            cells[2, 0].PutValue("Row 3");
            cells[5, 0].PutValue("Row 6");
            cells[9, 0].PutValue("Row 10");

            Console.WriteLine("Before deleting blank rows:");
            for (int i = 0; i <= 10; i++)
            {
                Console.WriteLine($"Row {i + 1}: {(cells[i, 0].Value ?? "empty")}");
            }

            // Eliminar filas en blanco comenzando desde el índice 4 (Fila 5) hasta el índice 7 (Fila 8)
            DeleteBlankOptions options = new DeleteBlankOptions();
            options.StartIndex = 4;
            options.EndIndex = 7;
            cells.DeleteBlankRows(options);

            Console.WriteLine("\nAfter deleting blank rows from Row 5 to Row 8:");
            for (int i = 0; i <= 7; i++)
            {
                Console.WriteLine($"Row {i + 1}: {(cells[i, 0].Value ?? "empty")}");
            }
        }
    }
}
```

### Ver también

* class [DeleteBlankOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


