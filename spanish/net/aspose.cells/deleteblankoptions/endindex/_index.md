---
title: "DeleteBlankOptions.EndIndex"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad DeleteBlankOptions. Especifica el índice final de fila/columna, inclusivo del rango a comprobar y eliminar filas/columnas en blanco. El valor predeterminado es 1 y 1 significa el rango máximo de todos los objetos, celdas, dibujos ... que deben revisarse"
type: docs
url: /es/net/aspose.cells/deleteblankoptions/endindex/
---
## DeleteBlankOptions.EndIndex property

Especifica el índice final de fila/columna (inclusive) del rango a comprobar y eliminar filas/columnas en blanco. El valor predeterminado es -1 y -1 significa el rango máximo de todos los objetos (celdas, dibujos, ...) que deben verificarse.

```csharp
public int EndIndex { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DeleteBlankOptionsPropertyEndIndexDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Cells cells = wb.Worksheets[0].Cells;

            // Rellene algunas celdas con valores
            cells[0, 2].PutValue(2);
            cells[0, 5].PutValue(5);
            cells[0, 9].PutValue(9);

            // Cree opciones de eliminación con un rango específico
            DeleteBlankOptions dbo = new DeleteBlankOptions();
            dbo.StartIndex = 4;
            dbo.EndIndex = 7;

            // Elimine columnas en blanco dentro del rango especificado
            cells.DeleteBlankColumns(dbo);

            // Muestre los resultados para demostrar el efecto de EndIndex
            Console.WriteLine("Value at C1: " + cells[0, 2].IntValue);
            Console.WriteLine("Value at F1 (originally G1): " + cells[0, 4].IntValue);
            Console.WriteLine("Value at G1 (originally K1): " + cells[0, 6].IntValue);
        }
    }
}
```

### Ver también

* class [DeleteBlankOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


