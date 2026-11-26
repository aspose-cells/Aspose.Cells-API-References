---
title: "Cells.GetRowHeightInch"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Cells. Obtiene la altura de una fila especificada en unidades de pulgadas"
type: docs
url: /es/net/aspose.cells/cells/getrowheightinch/
---
## Cells.GetRowHeightInch method

Obtiene la altura de una fila especificada en unidades de pulgadas.

```csharp
public double GetRowHeightInch(int row)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fila | Int32 | Índice de fila |

### Valor de retorno

Altura de la fila

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodGetRowHeightInchWithInt32Demo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Establecer la altura de la fila en pulgadas para la fila 5
            cells.SetRowHeightInch(5, 1.5);

            // Obtener la altura de la fila en pulgadas para la fila 5
            double rowHeight = cells.GetRowHeightInch(5);

            // Mostrar el resultado
            Console.WriteLine("Row height in inches: " + rowHeight);
        }
    }
}
```

### Ver también

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


