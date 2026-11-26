---
title: "Cells.HideRow"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Cells. Oculta una fila"
type: docs
url: /es/net/aspose.cells/cells/hiderow/
---
## Cells.HideRow method

Oculta una fila.

```csharp
public void HideRow(int row)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fila | Int32 | Índice de fila. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodHideRowWithInt32Demo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ocultar fila 5
            worksheet.Cells.HideRow(5);
            
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


