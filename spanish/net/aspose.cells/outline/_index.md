---
title: "Clase Outline"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.Outline. Representa un esquema en una hoja de cálculo"
type: docs
url: /es/net/aspose.cells/outline/
---
## Outline class

Representa un contorno en una hoja de cálculo.

```csharp
public class Outline
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [SummaryColumnRight](../../aspose.cells/outline/summarycolumnright/) { get; set; } | Indica si la columna de resumen se posicionará a la derecha de las columnas de detalle en el esquema. |
| [SummaryRowBelow](../../aspose.cells/outline/summaryrowbelow/) { get; set; } | Indica si la fila de resumen se posicionará debajo de las filas de detalle en el esquema. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class OutlineDemo
    {
        public static void OutlineExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceda a la primera hoja de cálculo del libro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Accede al esquema de la hoja de cálculo
            Outline outline = worksheet.Outline;
            
            // Establece las propiedades del esquema
            outline.SummaryRowBelow = true; // Indicates if the summary row will be positioned below the detail rows
            outline.SummaryColumnRight = true; // Indicates if the summary column will be positioned to the right of the detail columns
            
            // Guarda el libro de trabajo
            workbook.Save("OutlineExample.xlsx");

            return;
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


