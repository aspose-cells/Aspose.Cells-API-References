---
title: "Worksheet.RemoveSplit"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método de Worksheet. Elimina la ventana dividida"
type: docs
url: /es/net/aspose.cells/worksheet/removesplit/
---
## Worksheet.RemoveSplit method

Elimina la ventana dividida.

```csharp
public void RemoveSplit()
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodRemoveSplitDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Dividir la hoja de cálculo
            worksheet.Split();
            Console.WriteLine("Worksheet split state: " + worksheet.PaneState);
            
            // Eliminar la división
            worksheet.RemoveSplit();
            Console.WriteLine("Worksheet split state after RemoveSplit: " + worksheet.PaneState);
            
            // Guarda el libro de trabajo
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ver también

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


