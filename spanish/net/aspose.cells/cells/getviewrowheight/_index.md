---
title: "Cells.GetViewRowHeight"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Cells. Obtiene la altura de una fila especificada"
type: docs
url: /es/net/aspose.cells/cells/getviewrowheight/
---
## Cells.GetViewRowHeight method

Obtiene la altura de una fila especificada.

```csharp
public double GetViewRowHeight(int row)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fila | Int32 | Índice de fila. |

### Valor de retorno

Altura de la fila.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodGetViewRowHeightWithInt32Demo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Establecer la altura de la fila 3 (en puntos)
            worksheet.Cells.SetRowHeight(3, 15);
            
            // Obtener la altura de vista de la fila 3
            double viewRowHeight = worksheet.Cells.GetViewRowHeight(3);
            
            // Mostrar el resultado
            Console.WriteLine("View Row Height for row 3: " + viewRowHeight);
        }
    }
}
```

### Ver también

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


