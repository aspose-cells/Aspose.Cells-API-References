---
title: "Cells.UnhideRow"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Cells. Desoculta una fila"
type: docs
url: /es/net/aspose.cells/cells/unhiderow/
---
## Cells.UnhideRow method

Muestra una fila.

```csharp
public void UnhideRow(int row, double height)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fila | Int32 | Índice de fila. |
| altura | Double | Altura de fila. La altura de la fila se cambiará solo cuando la fila esté oculta y el valor de altura proporcionado sea positivo. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodUnhideRowWithInt32DoubleDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ocultar fila 5
            worksheet.Cells.HideRow(5);
            
            // Mostrar fila 5 con una altura de 12.75
            worksheet.Cells.UnhideRow(5, 12.75);
            
            // Guarda el libro de trabajo
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ver también

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


