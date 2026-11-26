---
title: "Worksheet.FirstVisibleRow"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad de Worksheet. Representa el índice de la primera fila visible"
type: docs
url: /es/net/aspose.cells/worksheet/firstvisiblerow/
---
## Worksheet.FirstVisibleRow property

Representa el índice de la primera fila visible.

```csharp
public int FirstVisibleRow { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyFirstVisibleRowDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Establecer algunos datos de muestra
            for (int i = 0; i < 50; i++)
            {
                worksheet.Cells[i, 0].Value = "Row " + (i + 1);
            }
            
            // Establecer la primera fila visible en la fila 20
            worksheet.FirstVisibleRow = 20;
            
            // Mostrar la primera fila visible
            Console.WriteLine("First visible row: " + worksheet.FirstVisibleRow);
            
            // Guarda el libro de trabajo
            workbook.Save("FirstVisibleRowDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


