---
title: "Worksheet.FirstVisibleColumn"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Worksheet. Representa el índice de la primera columna visible"
type: docs
url: /es/net/aspose.cells/worksheet/firstvisiblecolumn/
---
## Worksheet.FirstVisibleColumn property

Representa el índice de la primera columna visible.

```csharp
public int FirstVisibleColumn { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyFirstVisibleColumnDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ocultar la primera columna (índice 0)
            worksheet.Cells.HideColumn(0);
            
            // Obtener y mostrar el índice de la primera columna visible
            Console.WriteLine("First visible column index: " + worksheet.FirstVisibleColumn);
            
            // Guarda el libro de trabajo
            workbook.Save("FirstVisibleColumnDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


